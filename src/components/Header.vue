<template>
  <header class="flex justify-between border-b border-slate-300 px-10 py-8">
    <div class="flex items-center gap-4">
      <img src="/logo.png" alt="logo" class="w-10 mr-5" />
      <div>
        <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Магазин лучших кроссовок</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img class="" src="/cart.svg" alt="cart" />
        <b>1205 руб.</b>
      </li>
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img class="" src="/heart.svg" alt="heart" />
        <span>Закладки</span>
      </li>
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img class="" src="/profile.svg" alt="profile" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>
