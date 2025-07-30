import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Calendar } from "lucide-react";
import Image from "next/image";

export default function CatalystLearningHub() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-sky-100 to-white text-gray-800 p-6">
      <header className="text-center mb-10">
        <div className="flex justify-center mb-4">
          <Image src="/logo-catalyst-learning-hub.png" alt="Catalyst Learning Hub Logo" width={100} height={100} />
        </div>
        <h1 className="text-4xl font-bold text-blue-800 mb-2">Catalyst Learning Hub</h1>
        <p className="text-lg text-gray-600">Igniting Minds, Transforming Futures</p>
      </header>

      <section className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-12">
        <Card className="bg-white shadow-xl rounded-2xl p-4">
          <CardContent>
            <h2 className="text-2xl font-semibold mb-2">🎓 Academic Tutoring</h2>
            <p className="text-gray-700">We offer high-quality tutoring for high school learners, with special focus on Life Sciences, Geography, and Mathematics.</p>
          </CardContent>
        </Card>

        <Card className="bg-white shadow-xl rounded-2xl p-4">
          <CardContent>
            <h2 className="text-2xl font-semibold mb-2">📚 Study Materials</h2>
            <p className="text-gray-700">Access our custom-made notes, past paper guides, and revision videos tailored for South African curricula.</p>
          </CardContent>
        </Card>

        <Card className="bg-white shadow-xl rounded-2xl p-4">
          <CardContent>
            <h2 className="text-2xl font-semibold mb-2">🌍 Online & In-Person Classes</h2>
            <p className="text-gray-700">Join flexible learning programs from anywhere in SA. Weekend classes available!</p>
          </CardContent>
        </Card>
      </section>

      <section className="text-center mb-10">
        <h2 className="text-3xl font-bold mb-4">Upcoming Programs</h2>
        <div className="flex flex-col items-center md:flex-row md:justify-center gap-6">
          <div className="flex items-center gap-3 bg-blue-100 px-4 py-3 rounded-xl shadow">
            <Calendar className="text-blue-700" />
            <div>
              <p className="text-blue-800 font-semibold">August 10, 2025</p>
              <p className="text-sm text-gray-600">Grade 12 Bootcamp - Johannesburg</p>
            </div>
          </div>
          <div className="flex items-center gap-3 bg-blue-100 px-4 py-3 rounded-xl shadow">
            <Calendar className="text-blue-700" />
            <div>
              <p className="text-blue-800 font-semibold">August 24, 2025</p>
              <p className="text-sm text-gray-600">Exam Strategy Webinar</p>
            </div>
          </div>
        </div>
      </section>

      <section className="text-center mb-12">
        <h2 className="text-3xl font-bold mb-4">Join Catalyst Learning Hub Today</h2>
        <p className="text-gray-700 mb-6">Let’s empower the next generation together. Whether you're a student or a parent, our doors are open for growth.</p>
        <Button className="text-white bg-blue-700 hover:bg-blue-800 px-6 py-2 text-lg rounded-xl">Get Started</Button>
      </section>

      <footer className="text-center text-sm text-gray-600 mt-10 border-t pt-6">
        <p>📧 Email: catalystlearninghub@gmail.com</p>
        <p>📞 Call/WhatsApp: 079 833 7377</p>
        <p>📺 YouTube: <a href="https://youtube.com/@CatalystLearningHub" target="_blank" className="text-blue-700 underline">@CatalystLearningHub</a></p>
        <p>📘 Facebook: <a href="https://facebook.com/@CatalystLearningHub" target="_blank" className="text-blue-700 underline">@Catalyst Learning Hub</a></p>
        <p className="mt-2">&copy; {new Date().getFullYear()} Catalyst Learning Hub. All rights reserved.</p>
      </footer>
    </div>
  );
}
