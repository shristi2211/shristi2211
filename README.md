type Developer struct {
    Role              string
    Specialization    []string
    CurrentFocus      string
    SystemsBuilt      int
    CoffeeConsumed    string
}

me := Developer{
    Role:           "Full Stack Developer @ RNR Consulting",
    Specialization: []string{"Distributed Systems", "Event-Driven Architecture", "Backend Engineering"},
    CurrentFocus:   "Building fault-tolerant systems that scale",
    SystemsBuilt:   "Production systems handling 120+ concurrent events",
    CoffeeConsumed: "Too much ☕",
}
