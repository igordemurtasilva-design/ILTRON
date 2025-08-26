export default function Home() {
  return (
    <main className="min-h-screen bg-gradient-to-b from-gray-900 to-black text-white font-sans">
      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center py-20 px-6">
        <h1 className="text-5xl font-bold mb-6">
          Potencialize seus resultados com a <span className="text-indigo-500">ILTRON</span>
        </h1>
        <p className="text-lg text-gray-300 max-w-2xl mb-8">
          Agência de marketing especializada em criativos de impacto, tráfego pago e presença digital estratégica para acelerar o crescimento do seu negócio.
        </p>
        <div className="flex flex-col md:flex-row gap-4">
          <a
            href="#contato"
            className="bg-indigo-600 hover:bg-indigo-700 px-8 py-4 rounded-2xl font-semibold text-lg shadow-lg transition"
          >
            Quero alavancar meu negócio
          </a>
          <a
            href="https://wa.me/5531987587431"
            target="_blank"
            rel="noopener noreferrer"
            className="bg-green-600 hover:bg-green-700 px-8 py-4 rounded-2xl font-semibold text-lg shadow-lg transition"
          >
            Fale no WhatsApp
          </a>
        </div>
      </section>

      {/* Services Section */}
      <section className="py-20 px-6 max-w-6xl mx-auto grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        <div className="bg-gray-800 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
          <h3 className="text-xl font-bold mb-4">Criativos para Divulgação</h3>
          <p className="text-gray-400">Designs atrativos e persuasivos que conectam sua marca ao público certo.</p>
        </div>
        <div className="bg-gray-800 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
          <h3 className="text-xl font-bold mb-4">Tráfego Pago</h3>
          <p className="text-gray-400">Campanhas estratégicas no Google, Meta e mais para maximizar resultados.</p>
        </div>
        <div className="bg-gray-800 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
          <h3 className="text-xl font-bold mb-4">Google Meu Negócio</h3>
          <p className="text-gray-400">Criação e otimização para garantir destaque nas buscas locais.</p>
        </div>
        <div className="bg-gray-800 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
          <h3 className="text-xl font-bold mb-4">Marketplace</h3>
          <p className="text-gray-400">Montamos sua loja online e posicionamos seus produtos em grandes marketplaces.</p>
        </div>
      </section>

      {/* Depoimentos */}
      <section className="py-20 px-6 bg-gray-950">
        <h2 className="text-3xl font-bold text-center mb-12">O que dizem nossos clientes</h2>
        <div className="max-w-4xl mx-auto grid md:grid-cols-2 gap-8">
          <div className="bg-gray-800 p-6 rounded-2xl shadow-lg">
            <p className="text-gray-300 mb-4">“A ILTRON transformou nossa presença online. As campanhas de tráfego pago geraram muito mais vendas do que esperávamos.”</p>
            <h4 className="font-semibold">— João Mendes, Loja de Roupas</h4>
          </div>
          <div className="bg-gray-800 p-6 rounded-2xl shadow-lg">
            <p className="text-gray-300 mb-4">“Graças à otimização no Google Meu Negócio, nossos clientes nos encontram com facilidade. O resultado foi imediato.”</p>
            <h4 className="font-semibold">— Ana Souza, Restaurante</h4>
          </div>
        </div>
      </section>

      {/* Formulário de Contato */}
      <section id="contato" className="py-20 px-6 text-center">
        <h2 className="text-4xl font-bold mb-6">Entre em contato com a ILTRON</h2>
        <p className="text-lg text-gray-300 mb-8">
          Preencha o formulário abaixo e nossa equipe retornará o mais rápido possível.
        </p>
        <form
          action="https://formspree.io/f/mblajdvd"
          method="POST"
          className="max-w-xl mx-auto bg-gray-800 p-8 rounded-2xl shadow-lg space-y-6"
        >
          <input
            type="text"
            name="nome"
            placeholder="Seu nome"
            required
            className="w-full p-3 rounded-lg text-black"
          />
          <input
            type="email"
            name="email"
            placeholder="Seu e-mail"
            required
            className="w-full p-3 rounded-lg text-black"
          />
          <input
            type="tel"
            name="whatsapp"
            placeholder="Seu WhatsApp"
            className="w-full p-3 rounded-lg text-black"
          />
          <textarea
            name="mensagem"
            placeholder="Digite sua mensagem"
            rows="5"
            required
            className="w-full p-3 rounded-lg text-black"
          ></textarea>
          <button
            type="submit"
            className="bg-indigo-600 hover:bg-indigo-700 px-8 py-4 rounded-2xl font-semibold text-lg shadow-lg transition w-full"
          >
            Enviar Mensagem
          </button>
        </form>
      </section>

      {/* Footer */}
      <footer className="bg-black py-6 text-center text-gray-500 text-sm">
        © {new Date().getFullYear()} ILTRON Marketing. Todos os direitos reservados.
      </footer>
    </main>
  );
}
