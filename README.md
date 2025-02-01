import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Calendar, Users, BookOpen, CreditCard, Image, MessageCircle, HelpCircle } from "lucide-react";
import Navbar from "@/components/Navbar";
import Footer from "@/components/Footer";
import Link from "next/link";

export default function SchoolDashboard() {
  return (
    <div className="min-h-screen flex flex-col">
      <Navbar />
      <div className="p-6 space-y-6 flex-grow">
        <h1 className="text-2xl font-bold text-center">Bienvenue à l'École Islamique</h1>
        <p className="text-center text-gray-600">Une éducation de qualité avec des valeurs islamiques</p>
        
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mt-6">
          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <Users className="w-10 h-10 text-blue-500" />
              <div>
                <h2 className="text-lg font-semibold">Inscription</h2>
                <p className="text-sm text-gray-500">Inscrire un nouvel élève</p>
                <Link href="/inscription">
                  <Button className="mt-2">Inscrire</Button>
                </Link>
              </div>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <BookOpen className="w-10 h-10 text-green-500" />
              <div>
                <h2 className="text-lg font-semibold">Notes</h2>
                <p className="text-sm text-gray-500">Consulter les résultats</p>
                <Link href="/notes">
                  <Button className="mt-2">Voir</Button>
                </Link>
              </div>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <CreditCard className="w-10 h-10 text-red-500" />
              <div>
                <h2 className="text-lg font-semibold">Paiements</h2>
                <p className="text-sm text-gray-500">Effectuer un paiement</p>
                <Link href="/paiement">
                  <Button className="mt-2">Payer</Button>
                </Link>
              </div>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <Calendar className="w-10 h-10 text-yellow-500" />
              <div>
                <h2 className="text-lg font-semibold">Emploi du temps</h2>
                <p className="text-sm text-gray-500">Voir les horaires des cours</p>
                <Link href="/emploi-du-temps">
                  <Button className="mt-2">Consulter</Button>
                </Link>
              </div>
            </CardContent>
          </Card>
        </div>
        
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-6">
          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <Image className="w-10 h-10 text-purple-500" />
              <div>
                <h2 className="text-lg font-semibold">Galerie Photos</h2>
                <p className="text-sm text-gray-500">Voir les images de l'école</p>
                <Link href="/galerie">
                  <Button className="mt-2">Voir</Button>
                </Link>
              </div>
            </CardContent>
          </Card>
          
          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <MessageCircle className="w-10 h-10 text-indigo-500" />
              <div>
                <h2 className="text-lg font-semibold">Témoignages</h2>
                <p className="text-sm text-gray-500">Ce que disent nos parents et élèves</p>
                <Link href="/temoignages">
                  <Button className="mt-2">Lire</Button>
                </Link>
              </div>
            </CardContent>
          </Card>
          
          <Card>
            <CardContent className="flex items-center space-x-4 p-6">
              <HelpCircle className="w-10 h-10 text-teal-500" />
              <div>
                <h2 className="text-lg font-semibold">FAQ</h2>
                <p className="text-sm text-gray-500">Réponses aux questions fréquentes</p>
                <Link href="/faq">
                  <Button className="mt-2">Consulter</Button>
                </Link>
              </div>
            </CardContent>
          </Card>
        </div>
      </div>
      <Footer />
    </div>
  );
}
# site-d-cole-
