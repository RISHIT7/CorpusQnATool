API_KEY := "AIzaSyD1J9Q1Q"

run: tester.out
	@./tester.out $(API_KEY)

tester.out: tester.cpp qna_tool.cpp Node.cpp
	@g++ tester.cpp qna_tool.cpp Node.cpp -o tester.out

clean:
	@rm -f tester.out
