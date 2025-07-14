
import { Badge } from "@/components/ui/badge";
import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { 
  Github, 
  Linkedin, 
  Mail, 
  MapPin, 
  Calendar,
  Award,
  Code,
  Database,
  Cloud,
  Server,
  Briefcase,
  GraduationCap,
  Trophy,
  ExternalLink
} from "lucide-react";

const Index = () => {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 via-white to-purple-50 p-6">
      <div className="max-w-4xl mx-auto space-y-8">
        {/* Header */}
        <div className="text-center mb-12">
          <div className="relative inline-block">
            <h1 className="text-6xl font-bold bg-gradient-to-r from-blue-600 via-purple-600 to-teal-600 bg-clip-text text-transparent mb-4">
              👋 Hello, I'm Firoz Khan
            </h1>
            <div className="absolute -top-2 -right-2 animate-bounce">
              <span className="text-2xl">🚀</span>
            </div>
          </div>
          <p className="text-xl text-gray-600 font-medium mb-6">
            Computer Science Student | Full-Stack Developer | DevOps Enthusiast
          </p>
          <div className="flex flex-wrap justify-center gap-4 text-gray-600">
            <div className="flex items-center gap-2">
              <MapPin className="w-4 h-4" />
              <span>Bengaluru, India</span>
            </div>
            <div className="flex items-center gap-2">
              <Mail className="w-4 h-4" />
              <span>hello.firozkhan@outlook.com</span>
            </div>
          </div>
          <div className="flex justify-center gap-4 mt-6">
            <Button variant="outline" className="flex items-center gap-2">
              <Github className="w-4 h-4" />
              GitHub
            </Button>
            <Button variant="outline" className="flex items-center gap-2">
              <Linkedin className="w-4 h-4" />
              LinkedIn
            </Button>
          </div>
        </div>

        {/* About Me */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <span className="text-2xl">🚀</span>
              About Me
            </CardTitle>
          </CardHeader>
          <CardContent>
            <p className="text-gray-700 leading-relaxed">
              I'm a passionate Computer Science student with expertise in <strong>web development, cloud computing, and DevOps</strong>. 
              I love building scalable applications and solving real-world problems with technology. My goal is to contribute to 
              innovative projects while continuously expanding my skill set.
            </p>
          </CardContent>
        </Card>

        {/* Skills */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <span className="text-2xl">🛠</span>
              Skills
            </CardTitle>
          </CardHeader>
          <CardContent className="space-y-6">
            <div>
              <h3 className="flex items-center gap-2 font-semibold text-lg mb-3">
                <Code className="w-5 h-5 text-blue-600" />
                Web Development
              </h3>
              <div className="flex flex-wrap gap-2">
                {['HTML', 'CSS', 'JavaScript', 'React', 'Node.js'].map(skill => (
                  <Badge key={skill} variant="secondary" className="px-3 py-1">
                    {skill}
                  </Badge>
                ))}
              </div>
            </div>
            
            <div>
              <h3 className="flex items-center gap-2 font-semibold text-lg mb-3">
                <Server className="w-5 h-5 text-green-600" />
                Programming Languages
              </h3>
              <div className="flex flex-wrap gap-2">
                {['Java', 'Python', 'C', 'SQL'].map(skill => (
                  <Badge key={skill} variant="secondary" className="px-3 py-1">
                    {skill}
                  </Badge>
                ))}
              </div>
            </div>
            
            <div>
              <h3 className="flex items-center gap-2 font-semibold text-lg mb-3">
                <Database className="w-5 h-5 text-purple-600" />
                Database Management
              </h3>
              <div className="flex flex-wrap gap-2">
                {['MySQL', 'MongoDB', 'DynamoDB'].map(skill => (
                  <Badge key={skill} variant="secondary" className="px-3 py-1">
                    {skill}
                  </Badge>
                ))}
              </div>
            </div>
            
            <div>
              <h3 className="flex items-center gap-2 font-semibold text-lg mb-3">
                <Cloud className="w-5 h-5 text-orange-600" />
                Cloud & DevOps
              </h3>
              <div className="flex flex-wrap gap-2">
                {['AWS (Lambda, S3)', 'Google Cloud', 'Docker', 'GitHub'].map(skill => (
                  <Badge key={skill} variant="secondary" className="px-3 py-1">
                    {skill}
                  </Badge>
                ))}
              </div>
            </div>
          </CardContent>
        </Card>

        {/* Education */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <GraduationCap className="w-6 h-6" />
              Education
            </CardTitle>
          </CardHeader>
          <CardContent className="space-y-4">
            <div className="border-l-4 border-blue-500 pl-4">
              <h3 className="font-semibold text-lg">BNM Institute of Technology</h3>
              <p className="text-gray-600 flex items-center gap-2">
                <Calendar className="w-4 h-4" />
                2022 - Present
              </p>
              <p className="text-gray-700">B.E. in Computer Science & Engineering (CGPA: 8.08)</p>
            </div>
            
            <div className="border-l-4 border-green-500 pl-4">
              <h3 className="font-semibold text-lg">Kendriya Vidyalaya No.1 Jalahalli (West)</h3>
              <p className="text-gray-600 flex items-center gap-2">
                <Calendar className="w-4 h-4" />
                2022
              </p>
              <p className="text-gray-700">12th Grade - Science (77.6%)</p>
            </div>
            
            <div className="border-l-4 border-purple-500 pl-4">
              <h3 className="font-semibold text-lg">Kendriya Vidyalaya No.1 AFS Bhui</h3>
              <p className="text-gray-600 flex items-center gap-2">
                <Calendar className="w-4 h-4" />
                2020
              </p>
              <p className="text-gray-700">10th Grade (81.8%)</p>
            </div>
          </CardContent>
        </Card>

        {/* Experience */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <Briefcase className="w-6 h-6" />
              Experience
            </CardTitle>
          </CardHeader>
          <CardContent className="space-y-6">
            <div className="border-l-4 border-blue-500 pl-4">
              <div className="flex justify-between items-start mb-2">
                <h3 className="font-semibold text-lg">Appzera | Python Developer Intern</h3>
                <span className="text-sm text-gray-500">March 2025 - June 2025</span>
              </div>
              <ul className="text-gray-700 space-y-1">
                <li>• Developed a <strong>chatbot</strong> using Python, PyQt (UI), and DeepSeek (NLP)</li>
                <li>• Enhanced conversational flows and performance optimization</li>
              </ul>
            </div>
            
            <div className="border-l-4 border-green-500 pl-4">
              <div className="flex justify-between items-start mb-2">
                <h3 className="font-semibold text-lg">Appteknow | DevOps Intern</h3>
                <span className="text-sm text-gray-500">August 2024 - September 2024</span>
              </div>
              <ul className="text-gray-700 space-y-1">
                <li>• Deployed <strong>serverless applications</strong> using AWS Lambda and S3</li>
                <li>• Automated cloud workflows with <strong>encryption layers</strong> for secure file management</li>
              </ul>
            </div>
            
            <div className="border-l-4 border-purple-500 pl-4">
              <div className="flex justify-between items-start mb-2">
                <h3 className="font-semibold text-lg">Bharat Intern | Web Developer Intern</h3>
                <span className="text-sm text-gray-500">July 2024 - August 2024</span>
              </div>
              <ul className="text-gray-700 space-y-1">
                <li>• Built <strong>web applications</strong> with HTML, CSS, and JavaScript</li>
                <li>• Improved <strong>user experience</strong> and front-end responsiveness</li>
              </ul>
            </div>
          </CardContent>
        </Card>

        {/* Certifications */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <Award className="w-6 h-6" />
              Certifications
            </CardTitle>
          </CardHeader>
          <CardContent>
            <div className="grid grid-cols-1 md:grid-cols-2 gap-3">
              {[
                'Red Hat System Administration - Red Hat',
                'Samsung Prism Python Programming - Samsung Innovation Campus',
                'Google Cloud Study Jam - Google Developer Student Clubs',
                'Prompt Engineering - Udemy'
              ].map((cert, index) => (
                <div key={index} className="flex items-center gap-2 p-2 rounded-lg bg-gray-50">
                  <Award className="w-4 h-4 text-yellow-500" />
                  <span className="text-sm">{cert}</span>
                </div>
              ))}
            </div>
          </CardContent>
        </Card>

        {/* Achievements */}
        <Card className="shadow-lg border-0 bg-white/80 backdrop-blur-sm">
          <CardHeader>
            <CardTitle className="flex items-center gap-2 text-2xl">
              <Trophy className="w-6 h-6" />
              Achievements & Extracurriculars
            </CardTitle>
          </CardHeader>
          <CardContent>
            <div className="space-y-2">
              <div className="flex items-center gap-2">
                <Trophy className="w-4 h-4 text-gold-500" />
                <span><strong>Codethon Participant</strong> - BMSCE Phase Shift 2024</span>
              </div>
              <div className="flex items-center gap-2">
                <Trophy className="w-4 h-4 text-gold-500" />
                <span><strong>Hackathon Participant</strong> - SIH 2024</span>
              </div>
            </div>
          </CardContent>
        </Card>

        {/* Footer */}
        <Card className="shadow-lg border-0 bg-gradient-to-r from-blue-600 to-purple-600 text-white">
          <CardContent className="text-center py-8">
            <h2 className="text-2xl font-bold mb-4">📬 Let's Connect!</h2>
            <p className="mb-6">I'm always open to collaborations and new opportunities. Feel free to reach out!</p>
            <div className="flex flex-wrap justify-center gap-4">
              <Button variant="secondary" className="flex items-center gap-2">
                <Mail className="w-4 h-4" />
                hello.firozkhan@outlook.com
              </Button>
              <Button variant="secondary" className="flex items-center gap-2">
                <Github className="w-4 h-4" />
                github.com/firozzorif
              </Button>
              <Button variant="secondary" className="flex items-center gap-2">
                <Linkedin className="w-4 h-4" />
                linkedin.com/in/firozzorif
              </Button>
            </div>
            <p className="mt-6 text-lg">⭐ <strong>Thanks for visiting my profile!</strong> ⭐</p>
          </CardContent>
        </Card>

        {/* Tech Stack Badges */}
        <div className="text-center">
          <h3 className="text-xl font-semibold mb-4">🔹 Tech Stack</h3>
          <div className="flex flex-wrap justify-center gap-3">
            {[
              { name: 'HTML5', color: 'bg-orange-500' },
              { name: 'CSS3', color: 'bg-blue-500' },
              { name: 'JavaScript', color: 'bg-yellow-500' },
              { name: 'Python', color: 'bg-blue-600' },
              { name: 'React', color: 'bg-cyan-500' },
              { name: 'Node.js', color: 'bg-green-600' },
              { name: 'AWS', color: 'bg-orange-600' },
              { name: 'Docker', color: 'bg-blue-700' }
            ].map(tech => (
              <Badge key={tech.name} className={`${tech.color} text-white px-3 py-1 text-sm font-medium`}>
                {tech.name}
              </Badge>
            ))}
          </div>
        </div>

        {/* Copy Instructions */}
        <Card className="shadow-lg border-2 border-dashed border-blue-300 bg-blue-50">
          <CardContent className="text-center py-6">
            <h3 className="text-lg font-semibold text-blue-800 mb-2">📋 How to Use This README</h3>
            <p className="text-blue-700 mb-4">
              This is a preview of your GitHub README. To use it, you'll need to convert this visual layout to Markdown format.
            </p>
            <Button className="bg-blue-600 hover:bg-blue-700">
              <ExternalLink className="w-4 h-4 mr-2" />
              View Markdown Version
            </Button>
          </CardContent>
        </Card>
      </div>
    </div>
  );
};

export default Index;
