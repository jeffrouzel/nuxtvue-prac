<script setup>
import { ref } from 'vue';

const users = ref([
    { id: 1, companyname: "Central Luzon College of Science and Technology" },
    { id: 2, companyname: "STI College" },
    { id: 3, companyname: "College of Maritime Leadership Innovation" },
    { id: 4, companyname: "PCI Tech Center Inc." },
    { id: 5, companyname: "Concentrix" },
    { id: 6, companyname: "HySeas III"},
    { id: 7, companyname: "Kongsberg" },
    { id: 8, companyname: "Maritime Merchant Marine Academy Graduate School" },
    { id: 9, companyname: "Hukbong Dagat Philippines" },
    { id: 10, companyname: "Inter-Global College Foundation Inc." },
    { id: 11, companyname: "Baliwag Maritime Academy" },
]);
</script>


<template>
    <div> User Management </div>

    <div class="overflow-hidden rounded-lg border border-gray-200 shadow-md">
        <table class="w-full border-collapse bg-white text-left text-sm text-gray-500">
            <thead class="bg-gray-50">
                <th scope="col" class="px-6 py-4 font-medium text-gray-900">Company Name</th>
            </thead>

            <tbody>
                <tr v-for="user in users" :key="user.id" class="hover:bg-gray-50">
                    <td class="px-5">
                    <NuxtLink :to="'/user/' + user.id" class="hover:text-blue-500 flex items-center space-x-3">
                        <td><IconsSampleCompany/></td>
                        <td class="px-3">{{ user.companyname }}</td>
                    </NuxtLink>
                    </td>          
                </tr>
            </tbody>
        </table>
    </div>
</template>
