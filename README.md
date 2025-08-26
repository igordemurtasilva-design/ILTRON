export default function LandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-black via-zinc-900 to-zinc-800 text-white font-sans">
      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center py-20 px-6">
        <h1 className="text-5xl font-bold mb-6">
          <span className="text-yellow-400">ILTRON</span> – Potencialize seu Negócio
        </h1>
        <p className="text-lg max-w-2xl mb-8">
          Ajudamos empresas a vender mais através de estratégias digitais: criativos impactantes,
          tráfego pago, otimização do Google Meu Negócio e muito mais.
        </p>
        <a
          href="#contato"
          className="bg-yellow-400 text-black px-6 py-3 rounded-2xl font-semibold hover:bg-yellow-300 transition"
        >
          Quero Vender Mais
        </a>
      </section>

      {/* Serviços */}
      <section className="grid md:grid-cols-2 lg:grid-cols-4 gap-8 px-10 py-20 bg-zinc-900">
        <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
          <h3 className="text-xl font-bold mb-3">🎨 Criativos para Divulgação</h3>
          <p>Designs modernos e persuasivos para suas campanhas chamarem atenção e converterem mais.</p>
        </div>
        <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
          <h3 className="text-xl font-bold mb-3">🚀 Tráfego Pago</h3>
          <p>Gestão estratégica de anúncios no Google, Instagram e Facebook para gerar resultados reais.</p>
        </div>
        <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
          <h3 className="text-xl font-bold mb-3">📍 Google Meu Negócio</h3>
          <p>Criação e otimização do seu perfil para aumentar a visibilidade e atrair clientes locais.</p>
        </div>
        <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
          <h3 className="text-xl font-bold mb-3">🛒 Loja em Marketplace</h3>
          <p>Montamos sua loja em grandes marketplaces e otimizamos para gerar vendas consistentes.</p>
        </div>
      </section>

      {/* Prova Social */}
      <section className="py-20 px-10 text-center">
        <h2 className="text-3xl font-bold mb-6">Resultados que Falam por Si</h2>
        <p className="max-w-2xl mx-auto mb-10">
          Nossos clientes aumentaram em média <span className="text-yellow-400 font-semibold">+70% nas vendas</span> após aplicar nossas estratégias digitais.
        </p>
        <div className="grid md:grid-cols-3 gap-8">
          <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
            <h3 className="text-2xl font-bold text-yellow-400">+500%</h3>
            <p>de aumento em engajamento</p>
          </div>
          <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
            <h3 className="text-2xl font-bold text-yellow-400">+300</h3>
            <p>clientes satisfeitos</p>
          </div>
          <div className="bg-zinc-800 p-6 rounded-2xl shadow-lg">
            <h3 className="text-2xl font-bold text-yellow-400">+1M</h3>
            <p>em faturamento gerado</p>
          </div>
        </div>
      </section>

      {/* Formulário de Contato */}
      <section id="contato" className="bg-yellow-400 text-black py-20 px-10 text-center">
        <h2 className="text-4xl font-bold mb-6">Solicite seu Orçamento</h2>
        <p className="mb-8 text-lg">
          Preencha o formulário abaixo e um especialista da ILTRON entrará em contato com você.
        </p>
        <form action="[https://formspree.io/f/mblajdvd]"method="POST" className="max-w-2xl mx-auto grid gap-6 text-left">
          <div>
            <label className="block mb-2 font-semibold">Nome</label>
            <input type="text" name="nome" placeholder="Seu nome" className="w-full p-3 rounded-lg border border-zinc-300" required />
          </div>
          <div>
            <label className="block mb-2 font-semibold">E-mail</label>
            <input type="email" name="email" placeholder="Seu e-mail" className="w-full p-3 rounded-lg border border-zinc-300" required />
          </div>
          <div>
            <label className="block mb-2 font-semibold">Telefone</label>
            <input type="tel" name="telefone" placeholder="Seu telefone" className="w-full p-3 rounded-lg border border-zinc-300" required />
          </div>
          <div>
            <label className="block mb-2 font-semibold">Observação para Orçamento</label>
            <textarea name="observacao" placeholder="Descreva sua necessidade..." className="w-full p-3 rounded-lg border border-zinc-300" rows="4"></textarea>
          </div>
          <button type="submit" className="bg-black text-yellow-400 px-6 py-3 rounded-2xl font-semibold hover:bg-zinc-800 transition">
            Enviar Solicitação
          </button>
        </form>

        <div className="mt-10">
          <a
            href="https://wa.me/553198758741"
            target="_blank"
            className="bg-green-500 text-white px-6 py-3 rounded-2xl font-semibold hover:bg-green-400 transition"
          >
            📲 Falar no WhatsApp
          </a>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-black text-center py-6 text-sm text-zinc-400">
        © {new Date().getFullYear()} ILTRON - Todos os direitos reservados.
      </footer>
    </div>
  );
}
