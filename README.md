class Coord:
        def __init__(self, x, y):
            self.x = x
            self.y = y
            
        def get(self):
            return (self.x, self.y)
        
        def add(self, other):
            return Coord(self.x + other.x, self.y + other.y)
        
c1 = Coord(1, 1)
c2 = Coord(2, 3)

c3 = c1.add(c2)
print(c3.get())

c4 = c3.add(c1)
print(c4.get())
