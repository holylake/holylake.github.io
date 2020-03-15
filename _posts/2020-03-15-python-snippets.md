
**argparse**

```python
def main():
	parser = argparse.ArgumentParser()
	
	parser.add_argument("echo", help="echo the string you use here")
	parser.add_argument("square", help="display a square of a given number",type=int,choices=[0, 1, 2,9,66])
	parser.add_argument('--input', '-i', help='The name of the color')
	parser.add_argument('-o', help='output')
	parser.add_argument('-d', action='store_true',help='debug')
	sys.argv=[sys.argv[0],'-o=out','sometext','2','-i=blue', '-d']
	
	#sys.argv=[sys.argv[0],'-o=out','sometext','66','-i=blue']
	
	args = parser.parse_args()
	print args.square**2
	print args.echo
	print args.o
	print(args.input)
	
	
	if args.d:
		print 'debug it!'
	return
```
