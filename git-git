#!/bin/bash
#
# For those days where you seem to constantly type "git git <cmd>"

speaketh() {
  for word in $1; do
    sleep 0.15
    echo -n "${word} "
  done
  echo ''
  sleep 1
}

speaketh "Brett: Git?"
speaketh "Jules: What country are you from?"
speaketh "Brett: Git? Git? G-git? - ?"
speaketh "Jules: \"Git\" ain't no country I've ever heard of. They speak English in Git?"
speaketh "Brett: Git?"
speaketh "Jules: English, motherfucker, do you speak it?"
speaketh "Brett: Yes! Yes!"
speaketh "Jules: Then you know what I'm sayin'!"
speaketh "Brett: Yes!"
speaketh "Jules: Describe what \"git ${@}\" looks like!"
speaketh "Brett: G-Git?"

speaketh "Jules: Say git again!"
speaketh "Jules: Say git again, I dare you,"
speaketh "Jules: I DOUBLE DARE YOU MOTHERFUCKER!"

for word in "Jules: SAY GIT ONE MORE GODDAMN TIME!"; do
  sleep 0.4
  echo -n "${word} "
done
echo

sleep 1
echo
sleep 1
echo
sleep 1

echo "Running \`git ${@}\`"
exec git $@
