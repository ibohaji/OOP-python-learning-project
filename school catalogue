class School:
  #The class school has 3 properties
  def __init__(self,name,level,numberOfStudents):
    self.name = name
    self.level = level
    self.numberOfStudents = numberOfStudents
  

  # Creating getters to return the value of each feature
  def get_name(self):
    return self.name
  def get_level(self):
    return self.level
  def get_numberOfStudents(self):
    return self.numberOfStudents
  
  def set_numberOfStudents(self,new_num):
    self.numberOfStudents = new_num
  
  def __repr__(self):
    return "A {} school named {} with {} students" %(self.name,self.level,self.numberOfStudents)
  

#Testing 
trefalke = School("Tre falke skolen","Primary",25)
print(trefalke.get_name(),"\n",trefalke.get_numberOfStudents(),"\n",trefalke.get_level())
trefalke.set_numberOfStudents(249)
print(trefalke.get_numberOfStudents())
  

class PrimarySchool(School):
  def __init__(self,name,numberOfStudents,pickupPolicy):
    super().__init__(name,"primary",numberOfStudents)
    self.pickupPolicy = pickupPolicy
  def get_pickupPolicy(self):
    return self.pickupPolicy
  def __repr__(self):
    parentRepr = super().__repr__()
    return parentRepr + "The pickup policy is: {}" %self.pickupPolicy

pickupPolicy = "No student should wait more than 20 min to be picked up"
bulowsvej = PrimarySchool("Bulowsvej",299,pickupPolicy)
print(bulowsvej.get_pickupPolicy())

class HighSchool(School):
  def __init__(self,name,numberOfStudents,sportsTeams):
    super().__init__(name,"High",numberOfStudents)
    self.sportsTeams = sportsTeams
  def get_sportsTeams(self):
    return self.sportsTeams
  def __repr__(self):
    parentRepr = super().__repr__()
    return parentRepr + "Available sports teams: {}"%self.sportsTeams

sports = ["Boxing","football","BasketBall","Wrestling","Gymnastics"]
Falkoner = HighSchool("Falkoner alle gym ",185,sports)

#Testing
print(Falkoner.get_sportsTeams())
