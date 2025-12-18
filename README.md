import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Gamepad2, Film, Music, Flame } from "lucide-react"; import { motion } from "framer-motion";

export default function GamingEntertainmentSite() { return ( <div className="min-h-screen bg-gradient-to-b from-black via-zinc-900 to-black text-white p-6"> {/* Header */} <header className="flex justify-between items-center mb-10"> <h1 className="text-3xl font-bold text-red-500">GameZone</h1> <nav className="space-x-6 text-sm"> <a className="hover:text-red-500" href="#games">Games</a> <a className="hover:text-red-500" href="#movies">Movies</a> <a className="hover:text-red-500" href="#music">Music</a> <a className="hover:text-red-500" href="#trending">Trending</a> </nav> </header>

{/* Hero Section */}
  <motion.section
    initial={{ opacity: 0, y: 40 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ duration: 0.6 }}
    className="text-center mb-14"
  >
    <h2 className="text-4xl font-extrabold mb-4">Gaming & Entertainment Hub</h2>
    <p className="text-zinc-400 max-w-xl mx-auto mb-6">
      Your one-stop destination for games, movies, music, and trending entertainment.
    </p>
    <Button className="bg-red-600 hover:bg-red-700 rounded-2xl px-8">
      Explore Now
    </Button>
  </motion.section>

  {/* Sections */}
  <div className="grid md:grid-cols-4 gap-6">
    <Card id="games" className="bg-zinc-900 rounded-2xl shadow-lg">
      <CardContent className="p-6 text-center">
        <Gamepad2 className="mx-auto mb-4 text-red-500" size={40} />
        <h3 className="text-xl font-semibold mb-2">Games</
