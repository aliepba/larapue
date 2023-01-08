<script>
    import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue'
    export default {
        components : {
            AuthenticatedLayout
        },
        props : {
            coa : [Object, Array]
        }
    }
</script>

<template>
    <Head title="Chart Of Accounts" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Chart Of Accounts</h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <a class="btn-add">Add New</a>
                <div class="bg-white overflow-hidden mt-2 shadow-sm sm:rounded-lg">
                    <table class="w-full text-sm text-left text-gray-500 dark:text-gray-400 lg:overflow-auto overflow-x-scroll">
                        <thead class="text-xs text-gray-700 uppercase bg-indigo-400 dark:bg-indigo-500 dark:text-white">
                            <tr>
                                <th scope="col" class="uppercase px-6 py-3">No</th>
                                <th scope="col" class="uppercase px-6 py-3">Name</th>
                                <th scope="col" class="uppercase px-6 py-3">Code</th>
                                <th scope="col" class="uppercase px-6 py-3">Type</th>
                                <th scope="col" class="uppercase px-6 py-3">Action</th>
                            </tr>
                        </thead>
                        <tbody>
                            <!-- <tr v-for="user, i in users" :key="user.id">
                                <td class="px-6 py-3">{{++i}}</td>
                                <td class="px-6 py-3">{{user.name}}</td>
                                <td class="px-6 py-3">{{user.email}}</td>
                                <td class="px-8 py-6">
                                    <a :href="route('user.edit', user.id)" class="btn-edit">Edit</a>
                                </td>
                            </tr> -->
                        </tbody>
                  </table>
                </div>
            </div>
        </div>

    </AuthenticatedLayout>
</template>
