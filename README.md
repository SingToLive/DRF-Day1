# DRF-Day1
DRF Day1 homework
 1. args, kwargs를 사용하는 예제 코드 짜보기


    def add(num):
      sum = 0
      for n in num:
          sum += n
      return sum

     def AddArgs(*num):
      sum = 0
      for n in num:
          sum += n
      return sum
      
      add(2,3,4,5,6)
      
      AddArgs(2,3,4,5,6)
      
      def Data(data):
        for k in data:
            print(f'{k} is key {data[k]} is value')
            
      
      def DataKWArgs(**data):
        for k in data:
            print(f'{k} is key {data[k]} is value')
            
      Data(hola='hopp', apple='mac')
      
      DataKWArgs(hola='hopp', apple='mac')
    
    

 2. mutable과 immutable은 어떤 특성이 있고, 어떤 자료형이 어디에 해당하는지 서술하기
    immutalbe 변경 불가능한 자료 Int, Str, Tuple
    
    mutable 변경 가능한 자료 List, Dict, ndarray

 3. DB Field에서 사용되는 Key 종류와 특징 서술하기
    Foregin Key : 다른 테이블을 참조할때 사용
    Unique Key : 중복 값 불허
    Primary Key : 테이블에서 반드시 존재, 두개 이상 존재 불가능, 중복값 불허, Foreign Key를 사용할때 참조할 테이블의 Primary Key를 바라봄

 4. django에서 queryset과 object는 어떻게 다른지 서술하기
    object = name, comment 등의 객체
    queryset은 데이터베이스에서 다양한 object를 가져온 집합
