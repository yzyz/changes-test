sh_test(
  name = "hellotest",
  srcs = ["moo/hello.sh"],
)

genrule(
  name = 'gentest',
  srcs = [],
  outs = ['testfile.sh'],
  cmd = 'echo "exit 0" > $@',
)

sh_test(
  name = 'fake_test',
  srcs = [':gentest'],
)
