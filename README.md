# Decorators_generators

1. Write retry decorator:
* Decorator should have following arguments : exceptions: tuple, tries: int, delay: int, backoff: int, logger: logging.Logger
* exceptions: tuple of exception in which cases function should be retried
* tries: how many times should function be retried
* delay: seconds interval between retries
* backoff multiplier e.g. value of 2 will double the delay each retry
* OPTIONAL: logger: logger to log retries 
     if you don't use logger just print following strings --> "Datetime :: Retrying <function_name> xth time!"  


Write rest of the following function and use to check decorator:

@retry(Exception, tries=3, delay=2, backoff=0,logger=None)
def random_numbers_interval(p, q):
 """ function generates rundom number in interval [0,1], p, q are from [0,1] interval
  ... 
  
  if random_number<p:
      raise Exception('less than lower bound')
  if random_number>q:
      raise Exception('grader than upper bound')
  ...

2. Create brutforce password generator that the passwords must have 
  * At least 8 characters—the more characters, the better.
  * A mixture of both uppercase and lowercase letters.
  * A mixture of letters and numbers.
  * Inclusion of at least one special character, e.g., ! @ # ? ] Note: do not use < or > in your password, as both can cause problems in Web browsers.
 Generator must have argument for password length. Use itertools functions.
 
 


  
