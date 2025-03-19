<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <script src="https://cdn.tailwindcss.com"></script>
  <title>Menu Responsivo</title>
</head>
<body class="bg-gray-900">
  <header class="bg-black p-4 flex justify-between items-center">
    <div class="text-white text-lg font-bold">Spotify</div>
    <nav class="hidden md:flex space-x-6 text-white">
      <a href="#" class="hover:text-gray-400">Premium</a>
      <a href="#" class="hover:text-gray-400">Suporte</a>
      <a href="#" class="hover:text-gray-400">Baixar</a>
      <span class="text-gray-500">|</span>
      <a href="#" class="hover:text-gray-400">Inscrever-se</a>
      <a href="#" class="hover:text-gray-400">Entrar</a>
    </nav>
    <button class="md:hidden text-white text-2xl" onclick="document.querySelector('#menu-modal').showModal()">
      ☰
    </button>
  </header>

  <dialog id="menu-modal" class="bg-black text-white w-3/4 max-w-sm p-4 rounded-lg">
    <form method="dialog">
      <button class="absolute top-2 right-4 text-white text-2xl">×</button>
    </form>
    <nav class="flex flex-col space-y-4 mt-6">
      <a href="#" class="hover:text-gray-400">Premium</a>
      <a href="#" class="hover:text-gray-400">Suporte</a>
      <a href="#" class="hover:text-gray-400">Baixar</a>
      <a href="#" class="border border-pink-500 px-4 py-2 text-center">Inscrever-se</a>
      <a href="#" class="bg-green-500 px-4 py-2 rounded text-center">Entrar</a>
    </nav>
  </dialog>
</body>
</html>
