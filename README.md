djangoTest
==========

new_django
class expr(object):
    def __init__(self,value = None, left = None, right = None):
        self.value = value
        self.left = left
        self.right= right

    def evaluate(self):
        if self.value == '+':
            return self.left.evaluate() + self.right.evaluate()
        elif self.value == '-':
            return self.left.evaluate()- self.right.evaluate()
        elif self.value == '*':
            return self.left.evaluate() * self.right.evaluate()
        elif self.value == '/':
            return self.left.evaluate()/self.right.evaluate()
        else:
            return self.value
        
