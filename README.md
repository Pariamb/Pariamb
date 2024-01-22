class dnode():
    def init(self,d):
        self.data=None 
        self.next=None 
        self.prev=None 
class dlinkedlist:
    def init(self):
        self.head=None 
    def display(self):
        t=self.head
        while(t!=None):
            print(t.data,end='<-->')
            t=t.next
        print(None)
    def addfirst(self,d):
        n=dnode(d)
        if self.head!=None:
            self.head=None 
            n.next=self.head
            self.head.prev=n 
                 l=dlinkedlist()
                 l.addfirst(5)
                 l.addfirst(6)
                 l.display()
#---------------------------------------------------------------------
class stack():
    def init(self,limit=2):
        self.stack=[] 
        self.limit=limit 
    def peak(self):
        if len(self.stak)<=0:
            return -1 
        else:
            return self.stack[len(self.stack)]
    def pop(self):
         if len(self.stak)<=0:
            return -1 
         else:
             return self.stack.pop()
    def push(self,data):
         if len(self.stack)>=self.limit:
             return -1
         else:
             self.stack.append(data) 
    def display(self):
         if len(self.stak)<=0:
            return -1 
         else:
             if i in self.stack:
                 print(i)
         l=stack() 
         l.peak(5)
         l.push(3)
         l.display


        

