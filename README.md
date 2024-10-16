
--->
import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import { Input } from "@/components/ui/input"
import { Textarea } from "@/components/ui/textarea"
import { Palette, Globe, FileText, Users, Zap, MapPin } from "lucide-react"

export default function Home() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-purple-100 to-indigo-200 dark:from-purple-900 dark:to-indigo-950">
      <header className="container mx-auto py-6">
        <nav className="flex justify-between items-center">
          <h1 className="text-2xl font-bold text-purple-800 dark:text-purple-300">S-Solutions by Makalane Ezile</h1>
          <div className="space-x-4">
            <Button variant="ghost">About</Button>
            <Button variant="ghost">Services</Button>
            <Button variant="ghost">Contact</Button>
          </div>
        </nav>
      </header>

      <main className="container mx-auto px-4 py-16">
        <section className="text-center mb-16">
          <h2 className="text-4xl font-bold mb-4 text-purple-900 dark:text-purple-100">Welcome to S-Solutions by Makalane Ezile</h2>
          <p className="text-xl mb-8 text-purple-800 dark:text-purple-200">High-quality graphic design services in Kokstad, South Africa</p>
          <Button size="lg" className="bg-purple-600 hover:bg-purple-700 text-white">Get Started</Button>
        </section>

        <section className="mb-16">
          <h3 className="text-2xl font-bold mb-8 text-center text-purple-800 dark:text-purple-200">Our Services</h3>
          <div className="grid md:grid-cols-3 gap-8">
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <Palette className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Posters</CardTitle>
              </CardHeader>
              <CardContent>
                <p>Eye-catching designs tailored to your needs, perfect for events, promotions, or branding.</p>
              </CardContent>
            </Card>
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <Globe className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Web Design</CardTitle>
              </CardHeader>
              <CardContent>
                <p>Custom websites that are not only beautiful but also functional, ensuring a seamless user experience.</p>
              </CardContent>
            </Card>
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <FileText className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Documentation</CardTitle>
              </CardHeader>
              <CardContent>
                <p>Professional documentation services to present your information clearly and effectively.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section className="mb-16">
          <h3 className="text-2xl font-bold mb-8 text-center text-purple-800 dark:text-purple-200">Why Choose Us?</h3>
          <div className="grid md:grid-cols-3 gap-8">
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <Users className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Personalized Approach</CardTitle>
              </CardHeader>
              <CardContent>
                <p>We take the time to understand your vision and goals, ensuring our designs align perfectly with your brand.</p>
              </CardContent>
            </Card>
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <Zap className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Quality & Creativity</CardTitle>
              </CardHeader>
              <CardContent>
                <p>Our designs are crafted with attention to detail, ensuring a unique and memorable result.</p>
              </CardContent>
            </Card>
            <Card className="bg-white/80 dark:bg-purple-900/80">
              <CardHeader>
                <MapPin className="w-12 h-12 mb-4 text-purple-600 dark:text-purple-400" />
                <CardTitle>Local Expertise</CardTitle>
              </CardHeader>
              <CardContent>
                <p>Being based in Kokstad allows us to connect with our community and understand local market needs.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section className="max-w-md mx-auto">
          <Card className="bg-white/90 dark:bg-purple-900/90">
            <CardHeader>
              <CardTitle>Contact Us</CardTitle>
              <CardDescription>Get in touch with our team of experts</CardDescription>
            </CardHeader>
            <CardContent>
              <form className="space-y-4">
                <Input placeholder="Your Name" />
                <Input type="email" placeholder="Your Email" />
                <Textarea placeholder="Your Message" />
                <Button type="submit" className="w-full bg-purple-600 hover:bg-purple-700 text-white">Send Message</Button>
              </form>
            </CardContent>
          </Card>
        </section>
      </main>

      <footer className="bg-purple-800 dark:bg-purple-950 text-white py-8 mt-16">
        <div className="container mx-auto text-center">
          <p>&copy; 2023 Solutions by Makalane Ezile. All rights reserved.</p>
          <div className="mt-4">
            <p>Email: ezilemakalne50@gmail.com</p>
            <p>Phone: +27 73 378 4177</p>
            <p>Location: Kokstad, South Africa</p>
          </div>
        </div>
      </footer>
    </div>
  )
}
