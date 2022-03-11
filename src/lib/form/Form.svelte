
<form class="p-6 flex flex-col justify-center" action="https://submit-form.com/F8kispbK">
    <div class="flex flex-col">
        <label for="name" class="hidden">Name</label>
        <input type="text" id="name" name="name" placeholder="Name" required="" class="w-100 mt-2 py-3 px-3 rounded-lg bg-white dark:bg-gray-800 border border-blue dark:border-gray-700 text-gray-800 font-semibold focus:border-blue-500 focus:outline-none" />
        <!-- <span class="text-xs text-red-700" id="fullNameHelp">Please provide a name.</span> -->
    </div>

    <div class="flex flex-col mt-2">
        <label for="email" class="hidden">Email</label>
        <input type="email" id="email" name="email" placeholder="Email" required="" class="w-100 mt-2 py-3 px-3 rounded-lg bg-white dark:bg-gray-800 border border-blue dark:border-gray-700 text-gray-800 font-semibold focus:border-blue-500 focus:outline-none" />
        <!-- <span class="text-xs text-green-700" id="emailHelp">Please provide a real email.</span> -->
    </div>

    <div class="flex flex-col mt-2">
        <label for="message" class="hidden">Message</label>
        <textarea id="message" name="message" required="" placeholder="What can I help you with?" class="w-100 mt-2 py-3 px-3 rounded-lg bg-white dark:bg-gray-800 border border-blue dark:border-gray-700 text-gray-800 font-semibold focus:border-blue-500 focus:outline-none" />
    </div>

    <button type="submit" class="font-bold py-3 px-6 rounded-lg mt-3 bg-orange text-white hover:opacity-80">
        Submit
    </button>
</form>