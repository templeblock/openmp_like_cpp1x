#env = Environment( CC = '/opt/local/bin/gcc', CXX = '/opt/local/bin/g++' )
env = Environment()

print "CC is:", env['CC']
print "CXX is:", env['CXX']

env.Append(CPPPATH = ['/opt/local/include/'])

env.Append(CPPFLAGS = ['-O3', '-std=c++11', '-pthread'])

env.Append(LIBPATH = ['/opt/local/lib/'])

env.Append(LIBS = ['pthread'])

#env.Append(LINKFLAGS = ['-Wl,--no-as-needed'])

t = env.Program(target='main', source=['./openmplike.cpp', './main.cpp'])

Default(t)
