    class MyProfile:
        def __init__(self, name, age, uni, field, interests):
            self.name = name
            self.age = age
            self.uni = uni
            self.field = field
            self.interests = interests.split(", ")

        def display_profile(self):
            intro_interests =self.interests[:2]
            extra_interests = ', '.join(self.interests[2:])
            print(f"""
            Hi! My name is {self.name} and I am {self.age} years old.
            I am a first year {self.field} student at {self.uni}.
            My main interests are {intro_interests[0]} and {intro_interests[1]}, 
            but in my free time I also like to {extra_interests}
            """)

    def main():
        me = MyProfile("Kinga", 20, "AGH University of Science and Technology", "ICT",
                       "programming, networks, powerlift, read science fiction books, listen to podcasts")
        me.display_profile()

    if __name__ == "__main__":
        main()
  


