package main

import (
	"fmt"
	"os"
)

func main() {
	dir, _ := os.UserHomeDir()
	for {
		var userInput int
		fmt.Println("1) Enable SteamVR\n2) Disable SteamVR\n3) Exit")
		_, _ = fmt.Scanln(&userInput)
		switch userInput {
		case 1:
			fmt.Println("SteamVR is now enabled.")
			err0 := os.Rename("C:\\Program Files (x86)\\Steam\\steamapps\\common\\SteamVR1", "C:\\Program Files (x86)\\Steam\\steamapps\\common\\SteamVR")
			err1 := os.Rename(dir+"\\AppData\\Local\\openvr1", dir+"\\AppData\\Local\\openvr")
			if err0 != nil || err1 != nil {
				print("ERROR: SteamVR is already enabled.\n")
			}
			break
		case 2:
			fmt.Println("SteamVR is now disabled.")
			err2 := os.Rename("C:\\Program Files (x86)\\Steam\\steamapps\\common\\SteamVR", "C:\\Program Files (x86)\\Steam\\steamapps\\common\\SteamVR1")
			err3 := os.Rename(dir+"\\AppData\\Local\\openvr", dir+"\\AppData\\Local\\openvr1")
			if err2 != nil || err3 != nil {
				print("ERROR: SteamVR is already disabled.\n")
			}
			break
		case 3:
			os.Exit(0)
		default:
			fmt.Println("Invalid input.")
		}
	}
}
