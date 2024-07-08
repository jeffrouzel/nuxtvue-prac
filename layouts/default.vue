<template>
  <div class="w-screen h-screen flex flex-col">
    <!-- Navbar -->
    <NavBar />
    <div class="h-[calc(100vh-80px)] flex">
      <!-- Sidebar -->
      <SideBar />
      <div class="w-screen h-screen px-24 py-16"><slot /></div>
    </div>
  </div>
</template>