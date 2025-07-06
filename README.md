# Bank_Account_Manager
class amount():
    def _init_(self,balance,acc):
        self.balance = balance
        self.acc = acc
#debit
    def debit(self,amount):
        self.balance -= amount
        print("the debited amount is :",amount)
        print("total balance",self.get_balance())
#credit
    def credit(self,amount):
        self.balance += amount
        print("the credited amount is :",amount)  
        print("total balance",self.get_balance())
#balance
    def get_balance(self):
        return self.balance    

Acc1 = amount(4500, 88002366598)         
Acc1.debit(1000)
Acc1.credit(500)
Acc1.get_balance()
print("the account number is :",Acc1.acc)
