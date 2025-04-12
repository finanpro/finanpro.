# finanpro.
Página de aterrizaje para FinanPro - Financiación para servicios".
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";

export default function LandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 to-red-50 p-8">
      <header className="mb-12 text-center">
        <h1 className="text-4xl font-bold text-blue-800">FinanPro</h1>
        <p className="text-lg text-gray-700 mt-2">
          Financing Solutions for Service-Based Businesses
        </p>
      </header>

      <section className="max-w-3xl mx-auto text-center mb-12">
        <h2 className="text-2xl font-semibold text-gray-800 mb-4">
          💼 Professional Financing for Your Clients
        </h2>
        <p className="text-gray-600 text-md">
          FinanPro helps service businesses like remodeling, HVAC, and painting offer flexible payment options to their clients — without the hassle.
        </p>
      </section>

      <section className="max-w-xl mx-auto">
        <Card className="shadow-xl">
          <CardContent className="p-6">
            <h3 className="text-xl font-semibold text-gray-800 mb-4 text-center">
              Get Started with FinanPro
            </h3>
            <form className="space-y-4">
              <div>
                <Label htmlFor="name">Full Name</Label>
                <Input id="name" placeholder="Your full name" />
              </div>
              <div>
                <Label htmlFor="business">Business Name</Label>
                <Input id="business" placeholder="Your company name" />
              </div>
              <div>
                <Label htmlFor="email">Email Address</Label>
                <Input id="email" type="email" placeholder="you@example.com" />
              </div>
              <div>
                <Label htmlFor="service">Type of Service</Label>
                <Input id="service" placeholder="e.g. Remodeling, HVAC, Painting" />
              </div>
              <Button className="w-full bg-blue-700 text-white hover:bg-blue-800">
                Submit Interest
              </Button>
            </form>
          </CardContent>
        </Card>
      </section>
    </div>
  );
}
