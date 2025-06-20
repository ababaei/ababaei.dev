<template>
  <canvas ref="canvas" class="absolute inset-0 -z-10 w-full h-full" />
</template>

<script setup>
import { onMounted, onBeforeUnmount, ref } from 'vue'

const canvas = ref(null)
let ctx
let animationId

let path = [{ x: 100, y: 100 }] // starting point
let dir_x = Math.random() * 2 * Math.PI
let dir_y = Math.random() * 2 * Math.PI
let length = 0

function drawDottedLine() {
    let wrapOccurred = false

    ctx.setLineDash([5, 10])
    ctx.lineWidth = 2
    ctx.strokeStyle = 'rgba(0, 0, 0, 0.8)'
    ctx.beginPath()
    ctx.moveTo(path[0].x, path[0].y)
    ctx.lineTo(path[path.length - 1].x, path[path.length - 1].y)
    ctx.stroke()
}

function animate() {
    ctx.fillStyle = 'rgba(255, 255, 255, 0.1)' // slight transparent fill for fade effect
    ctx.fillRect(0, 0, canvas.value.width, canvas.value.height)
  
  // Move forward
    const last = path[path.length - 1]
    const speed = 1
    let next = {
      x: last.x + Math.cos(dir_x) * speed,
      y: last.y + Math.sin(dir_y) * speed,
    }

    path.push(next)

    drawDottedLine()


    animationId = requestAnimationFrame(animate)
}

onMounted(() => {
    canvas.value.width = window.innerWidth
    canvas.value.height = window.innerHeight
    ctx = canvas.value.getContext('2d')

    animate()
})

onBeforeUnmount(() => {
    cancelAnimationFrame(animationId)
})
</script>