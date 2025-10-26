import { motion } from 'framer-motion'
import { Button } from '@/components/ui/button'
import { Card, CardContent } from '@/components/ui/card'
import { ShieldCheck, PackageSearch, LineChart, ShoppingBag } from 'lucide-react'

export default function VerifyGenius() {
  return (
    <div className="bg-gradient-to-b from-white to-gray-100 text-gray-900">
      {/* Hero Section */}
      <section className="text-center py-20 px-6 bg-gradient-to-r from-pink-500 to-purple-600 text-white">
        <motion.h1 initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.6 }} className="text-5xl font-extrabold mb-4">
          VerifyGenius.AI
        </motion.h1>
        <p className="text-lg max-w-2xl mx-auto mb-6">
          Revolutionizing fashion retail with AI-powered authenticity verification, return prediction, and transparent supply chains.
        </p>
        <Button size="lg" className="bg-white text-purple-600 hover:bg-gray-200 font-semibold">Get Started</Button>
      </section>

      {/* Problems Section */}
      <section className="py-16 px-8 max-w-6xl mx-auto text-center">
        <h2 className="text-3xl font-bold mb-10">The Fashion Industry Crisis</h2>
        <div className="grid md:grid-cols-3 gap-8">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-3">High Return Rates</h3>
              <p>1 in 3 online purchases are returned due to size mismatch, quality issues, and dissatisfaction.</p>
            </CardContent>
          </Card>
          <Card className="shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-3">Counterfeit Products</h3>
              <p>Nearly 10% of online sales are counterfeit, eroding brand trust and consumer confidence.</p>
            </CardContent>
          </Card>
          <Card className="shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-3">Supply Chain Opacity</h3>
              <p>Limited transparency leads to distrust and environmental waste across the fashion supply chain.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Solution Section */}
      <section className="py-16 bg-white px-8">
        <h2 className="text-3xl font-bold text-center mb-10">Our Solution: VerifyGenius.AI</h2>
        <div className="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
          <Card className="shadow-md">
            <CardContent className="p-6 text-center">
              <ShieldCheck className="w-10 h-10 text-purple-600 mx-auto mb-4" />
              <h3 className="text-xl font-semibold mb-2">AI Image Verification</h3>
              <p>Scan, analyze, and detect counterfeits using CNN-based image models in seconds.</p>
            </CardContent>
          </Card>
          <Card className="shadow-md">
            <CardContent className="p-6 text-center">
              <LineChart className="w-10 h-10 text-purple-600 mx-auto mb-4" />
              <h3 className="text-xl font-semibold mb-2">Return Prediction</h3>
              <p>Predict product return probability using customer behavior, reviews, and product data.</p>
            </CardContent>
          </Card>
          <Card className="shadow-md">
            <CardContent className="p-6 text-center">
              <PackageSearch className="w-10 h-10 text-purple-600 mx-auto mb-4" />
              <h3 className="text-xl font-semibold mb-2">Supply Chain Transparency</h3>
              <p>Track every product with blockchain-powered NFC/QR tags for verified traceability.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Impact Metrics */}
      <section className="py-20 bg-gray-50 text-center">
        <h2 className="text-3xl font-bold mb-10">Impact Metrics</h2>
        <div className="grid md:grid-cols-3 gap-8 max-w-4xl mx-auto">
          <div>
            <p className="text-5xl font-extrabold text-purple-600">40%</p>
            <p className="mt-2">Reduction in returns through predictive analytics.</p>
          </div>
          <div>
            <p className="text-5xl font-extrabold text-purple-600">60%</p>
            <p className="mt-2">Improvement in counterfeit detection accuracy.</p>
          </div>
          <div>
            <p className="text-5xl font-extrabold text-purple-600">50%</p>
            <p className="mt-2">Boost in customer trust and brand confidence.</p>
          </div>
        </div>
      </section>

      {/* Future Enhancements */}
      <section className="py-20 px-8 max-w-6xl mx-auto">
        <h2 className="text-3xl font-bold text-center mb-10">Future Enhancements</h2>
        <div className="grid md:grid-cols-3 gap-8">
          <Card className="shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">AI Virtual Try-On</h3>
              <p>Use AR fitting to reduce size mismatches and increase satisfaction.</p>
            </CardContent>
          </Card>
          <Card className="shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Federated Learning</h3>
              <p>Enable brands to collaborate on AI training without data sharing.</p>
            </CardContent>
          </Card>
          <Card className="shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Sustainability Dashboard</h3>
              <p>Monitor and reduce environmental impact through AI insights.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-10 bg-purple-700 text-white text-center">
        <ShoppingBag className="w-8 h-8 mx-auto mb-2" />
        <p className="text-lg font-semibold">VerifyGenius.AI</p>
        <p className="text-sm mt-2">Making fashion smarter, transparent, and sustainable.</p>
        <p className="text-xs mt-4">© 2025 VerifyGenius.AI. All rights reserved.</p>
      </footer>
    </div>
  )
}
