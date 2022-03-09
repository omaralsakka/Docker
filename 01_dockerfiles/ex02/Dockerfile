FROM ft-rails:on-build

EXPOSE 3000
CMD [ "rails" , "s", "-b", "0.0.0.0", "-p", "3000"]

#first  docker build -t ft-rails:on-build ft-rails in root
#second docker build -t omar/rails ./
#third docker run --rm -p 3000:3000 omar/rails