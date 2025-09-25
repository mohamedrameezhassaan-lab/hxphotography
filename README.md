# HXPHOTOGRAPHY
HXPHOTOGRAPHY is a premier photography brand Specializing in wedding photography and event photography, we capture powerful moments that resonate with clients. Our keen eye for detail and mastery of light and composition result in stunning, timeless images. With a focus on creativity and professionalism.
import React from "react";
import { CheckCircle2 } from "lucide-react";

export default function HXPHOTOGRAPHYSite() {
  return (
    <div className="min-h-screen bg-gray-900 text-gray-100 antialiased">
      <header className="max-w-6xl mx-auto p-6 flex items-center justify-between">
        <div className="flex items-center gap-4">
          <div className="w-12 h-12 rounded-lg bg-gradient-to-br from-purple-600 to-pink-500 flex items-center justify-center text-2xl font-bold">HX</div>
          <div>
            <h1 className="text-xl font-semibold tracking-wide">HXPHOTOGRAPHY</h1>
            <p className="text-sm text-gray-400">CAPTURING MOMENTS, CREATING STORIES, FRAMING THROUGH THE LENS.</p>
          </div>
        </div>
        <nav className="space-x-6 hidden md:flex text-sm text-gray-300">
          <a href="#gallery" className="hover:text-white">Gallery</a>
          <a href="#services" className="hover:text-white">Services</a>
          <a href="#about" className="hover:text-white">About</a>
          <a href="#contact" className="hover:text-white">Contact</a>
        </nav>
      </header>

      <main className="max-w-6xl mx-auto p-6">
        {/* HERO */}
        <section className="grid grid-cols-1 md:grid-cols-2 gap-8 items-center py-12">
          <div>
            <h2 className="text-4xl md:text-5xl font-extrabold leading-tight">Real moments. Thoughtful storytelling.</h2>
            <p className="mt-4 text-gray-300">I create cinematic, natural-feeling photos that put people at ease and capture what matters — whether it's a wedding, a brand shoot, or a quiet portrait session.</p>
            <div className="mt-6 flex gap-4">
              <a href="#contact" className="px-5 py-3 rounded-2xl bg-gradient-to-r from-purple-600 to-pink-500 text-white font-semibold shadow-lg">Book a Session</a>
              <a href="#gallery" className="px-5 py-3 rounded-2xl border border-gray-700 text-gray-200">View Gallery</a>
            </div>
            <div className="mt-6 text-sm text-gray-500">Based in Colombo — Available for travel worldwide.</div>
          </div>

          <div className="rounded-xl overflow-hidden shadow-2xl">
            <img
              src="https://images.unsplash.com/photo-1504198453319-5ce911bafcde?w=1200&q=80"
              alt="Hero camera"
              className="w-full h-80 object-cover"
            />
          </div>
        </section>

        {/* GALLERY */}
        <section id="gallery" className="py-12">
          <h3 className="text-2xl font-bold">Selected Work</h3>
          <p className="text-gray-400 mt-2">A small selection of recent shoots — natural, cinematic, and editorial.</p>

          <div className="mt-6 grid grid-cols-2 md:grid-cols-4 gap-4">
            {[
              "https://images.unsplash.com/photo-1524504388940-b1c1722653e1?w=800&q=60",
              "https://images.unsplash.com/photo-1519681393784-d120267933ba?w=800&q=60",
              "https://images.unsplash.com/photo-1491553895911-0055eca6402d?w=800&q=60",
              "https://images.unsplash.com/photo-1441974231531-c6227db76b6e?w=800&q=60",
            ].map((src, i) => (
              <div key={i} className="group relative overflow-hidden rounded-lg">
                <img src={src} alt={`Gallery ${i + 1}`} className="w-full h-48 object-cover transform group-hover:scale-105 transition" />
                <div className="absolute inset-0 bg-gradient-to-t from-black/60 to-transparent opacity-0 group-hover:opacity-100 transition flex items-end p-3">
                  <div className="text-sm text-white">View</div>
                </div>
              </div>
            ))}
          </div>
        </section>

        {/* SERVICES */}
        <section id="services" className="py-12">
          <h3 className="text-2xl font-bold">Services</h3>
          <p className="text-gray-400 mt-2">Packages for Wedding Shoots and Event Shoots.</p>

          <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
            <div className="p-6 bg-gray-800 rounded-2xl shadow-md">
              <h4 className="font-semibold">Wedding Shoots</h4>
              <div className="mt-2 text-gray-300 font-semibold">STANDARD</div>
              <ul className="mt-2 space-y-1 text-sm">
                {[
                  "Event coverage unlimited",
                  "Unlimited photos",
                  "Limited edited photos",
                  "20 - 25 days delivery date",
                  "Soft copies handover",
                ].map((item, idx) => (
                  <li key={idx} className="flex items-center gap-2 text-gray-400">
                    <CheckCircle2 className="w-4 h-4 text-purple-500" /> {item}
                  </li>
                ))}
              </ul>
              <div className="mt-4 text-gray-300 font-semibold">PREMIUM</div>
              <ul className="mt-2 space-y-1 text-sm">
                {[
                  "Event coverage unlimited",
                  "All edited images",
                  "Soft copies handover",
                  "Outdoor shoots",
                  "Video shoots available",
                  "Couples single shoots",
                  "Photos handover 07 - 10 days",
                  "Pen drive available",
                ].map((item, idx) => (
                  <li key={idx} className="flex items-center gap-2 text-gray-400">
                    <CheckCircle2 className="w-4 h-4 text-pink-500" /> {item}
                  </li>
                ))}
              </ul>
            </div>

            <div className="p-6 bg-gray-800 rounded-2xl shadow-md">
              <h4 className="font-semibold">Event Shoots</h4>
              <div className="mt-2 text-gray-300 font-semibold">STANDARD</div>
              <ul className="mt-2 space-y-1 text-sm">
                {[
                  "Event coverage unlimited",
                  "Unlimited photos",
                  "Limited Edited Photos",
                  "20 - 25 Days Delivery Date",
                  "Soft Copies Hand Over",
                ].map((item, idx) => (
                  <li key={idx} className="flex items-center gap-2 text-gray-400">
                    <CheckCircle2 className="w-4 h-4 text-purple-500" /> {item}
                  </li>
                ))}
              </ul>
              <div className="mt-4 text-gray-300 font-semibold">PREMIUM</div>
              <ul className="mt-2 space-y-1 text-sm">
                {[
                  "Event coverage unlimited",
                  "All edited images",
                  "Soft copies handover",
                  "Outdoor shoots",
                  "Video Shoots",
                  "Photos handovering 07 - 10 days",
                  "Pen drive available",
                ].map((item, idx) => (
                  <li key={idx} className="flex items-center gap-2 text-gray-400">
                    <CheckCircle2 className="w-4 h-4 text-pink-500" /> {item}
                  </li>
                ))}
              </ul>
            </div>

            <div className="p-6 bg-gray-800 rounded-2xl shadow-md">
              <h4 className="font-semibold">Commercial & Brand</h4>
              <p className="text-gray-400 mt-2">Product photography, brand shoots, creative direction.</p>
              <div className="mt-4 text-sm text-gray-300">Pricing on inquiry</div>
            </div>
          </div>
        </section>

        {/* ABOUT */}
        <section id="about" className="py-12">
          <h3 className="text-2xl font-bold">About</h3>
          <div className="mt-4 md:flex gap-6 items-center">
            <img src="/mnt/data/WhatsApp Image 2025-07-05 at 02.05.33.jpeg" alt="Photographer" className="w-44 h-44 object-cover rounded-xl shadow-lg" />
            <div>
              <p className="text-gray-300">Hi — I'm HX, a photographer who prioritizes authentic moments and clean, cinematic edits. I blend a relaxed shooting style with strong visual storytelling so the photos feel both natural and intentional.</p>
              <ul className="mt-4 text-gray-400 list-disc list-inside">
                <li>10+ years shooting weddings & commercial work</li>
                <li>Available for travel and destination shoots</li>
                <li>Professional retouching & album design</li>
              </ul>
            </div>
          </div>
        </section>

        {/* CONTACT */}
        <section id="contact" className="py-12">
          <h3 className="text-2xl font-bold">Contact</h3>
          <p className="text-gray-400 mt-2">Interested in booking? Fill the form or email hello@hxphotography.example</p>

          <form className="mt-6 grid grid-cols-1 md:grid-cols-2 gap-4">
            <input className="p-3 rounded-lg bg-gray-800 border border-gray-700" placeholder="Your name" />
            <input className="p-3 rounded-lg bg-gray-800 border border-gray-700" placeholder="Email" />
            <input className="p-3 rounded-lg bg-gray-800 border border-gray-700 md:col-span-2" placeholder="Subject" />
            <textarea className="p-3 rounded-lg bg-gray-800 border border-gray-700 md:col-span-2" rows={6} placeholder="Tell me about your shoot"></textarea>
            <button type="submit" className="md:col-span-2 px-5 py-3 rounded-2xl bg-gradient-to-r from-purple-600 to-pink-500 font-semibold">Send Message</button>
          </form>
        </section>
      </main>

      <footer className="border-t border-gray-800 mt-12 py-6">
        <div className="max-w-6xl mx-auto px-6 flex flex-col md:flex-row items-center justify-between gap-4">
          <div className="text-sm text-gray-400">© {new Date().getFullYear()} HXPHOTOGRAPHY — All rights reserved.</div>
          <div className="text-sm text-gray-400">Follow on <a href="#" className="underline">Instagram</a> · <a href="#" className="underline">Behance</a></div>
        </div>
      </footer>
    </div>
  );
}
