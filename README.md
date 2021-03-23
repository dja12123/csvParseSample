# csvParseSample
충북대학교 자바프로그래밍 2021-1 과제 1 샘플

CSV파일을 단 4줄로 DTO로 만드는 방법

FileWriter writer = new FileWriter(file);

StatefulBeanToCsv<EarthQuakeData> beanToCsv = new StatefulBeanToCsvBuilder<EarthQuakeData>(writer).build();

beanToCsv.write(this.data.iterator());

writer.close();
