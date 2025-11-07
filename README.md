<div style="display: flex; justify-content: center; margin-top: 50px;">
  <h1 style="font-family: Arial, sans-serif; font-weight: 700; display: flex; align-items: center; gap: 10px;">
    <span>Systems Analyst and Developer</span>
     <img width="48" height="48" src="https://github.com/user-attachments/assets/08b3b127-0aff-410e-ac2e-76bbbea8d718" alt="Image">
  </h1>
<!-- GIF de código binário fixo no lado direito da tela -->
<div class="binary-gif" aria-hidden="true">
  <img
    src="https://media.giphy.com/media/3o7aD2saalBwwftBIY/giphy.gif"
    alt=""
    class="binary-gif__img"
  />
</div>

<style>
/* Container fixo no lado direito, centralizado verticalmente */
.binary-gif {
  position: fixed;
  right: 16px;
  top: 50%;
  transform: translateY(-50%);
  z-index: 9999;
  pointer-events: none;        /* não atrapalha cliques na página */
  display: block;
  user-select: none;
}

/* Estilo da imagem — ajuste width para controlar o tamanho */
.binary-gif__img {
  width: 240px;                /* tamanho padrão (mude para 180px, 300px, etc.) */
  max-width: 22vw;            /* responsivo relativo à largura da tela */
  height: auto;
  display: block;
  border-radius: 8px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.35);
  border: 1px solid rgba(255,255,255,0.06);
  background: rgba(0,0,0,0.18);
  backdrop-filter: blur(4px);
}

/* Em telas pequenas, escondemos para não cobrir conteúdo importante */
@media (max-width: 700px) {
  .binary-gif { display: none; }
}
</style>

