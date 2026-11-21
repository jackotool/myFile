package myFile

import (
	"errors"
	"os"
)

func FileExists(path string) (bool, error) {
	_, err := os.Lstat(path)
	if err != nil {
		if errors.Is(err, os.ErrNotExist) {
			return false, nil
		}
	}

	return true, nil
}
