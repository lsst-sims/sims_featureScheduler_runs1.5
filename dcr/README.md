Trying out forcing high airmass observations on both east and west

To run things in parallel, try

cat run_local.sh | xargs -n 33 -I'{}' -P2 bash -c '{}'
