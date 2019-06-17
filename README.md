# string-format-easy
String.format function for javascript modified from [luci2](https://git.openwrt.org/?p=project/luci2/ui.git).

# Code Example
%d

	'%d'.format(10) === '10'
	'%d, %d'.format(5, 10) === '5, 10'
	'%5d'.format(123) === '  123'
	'%-5d'.format(123) === '123  '
	'%05d'.format(123) === '00123'

%s

	'This is a %s'.format('pen') === 'This is a pen'
	'This is %s %s'.format('a', 'pen') === 'This is a pen'
	'%5s'.format('abc') === '  abc'
	'%-5s'.format('abc') === 'abc  '

%o

	'123 => %o'.format(123) === '123 => 173'
	'0x7b => %o'.format(0x7b) === '0x7b => 173'

%b

	'123 => %b'.format(123) === '123 => 1111011'
	'0x7b => %b'.format(0x7b) === '0x7b => 1111011'

%x

	'123 => %x'.format(123) === '123 => 7b'

%X

	'123 => %X'.format(123) === '123 => 7B'

%c

	'%c'.format(97) === 'a'
	'%c'.format(0x61) === 'a'

%f

	'%f'.format(1.12345) === '1.12345'
	'%.2f'.format(1.12345) === '1.12'

%t

	'%t'.format(13124) === '3h 38m 44s'

%m

	'%m'.format(1212) === '1.21 K'
	'%1024m'.format(1212) === '1.18 K'
	'%1024.1mB'.format(1212) === '1.2 KB'
