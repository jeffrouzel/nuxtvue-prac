<script setup lang="ts"></script>

<template>
  <div
    class="flex flex-col w-[250px] h-screen border-r-2 text-xs font-semibold text-gray-500 items-left pl-4"
  >
    <div class="flex flex-col items-center gap-2 pb-6">
      <IconsProfileIcon />
      <h1>SAN JUAN</h1>
      <h1>Super Admin</h1>
    </div>

    <div class="flex items-center gap-2 hover:text-blue-500 h-10">
      <IconsClientManagementIcon />
      <NuxtLink to="/">Client Management</NuxtLink>
    </div>

    <div class="flex items-center gap-2 hover:text-blue-500 h-10">
      <IconsUserManagementIcon />
      <NuxtLink to="/user-management">User Management</NuxtLink>
    </div>

    <div class="flex items-center gap-2 hover:text-blue-500 h-10">
      <IconsAuditIcon />
      <NuxtLink to="/audit">Audit</NuxtLink>
    </div>

    <div class="flex items-center gap-2 hover:text-blue-500 h-10">
      <IconsDataManagementIcon />
      <NuxtLink to="/data-management">Data Management</NuxtLink>
    </div>

    <div class="flex items-center gap-2 hover:text-blue-500 h-10">
      <IconsConfigIcon />
      <NuxtLink to="/configuration">Configuration</NuxtLink>
    </div>
    
  </div>
</template>
