[RealEstate Design.zip](https://github.com/Mahesh-Ingavale/Web-Development/files/6643846/RealEstate.Design.zip)
# Web-Development 
# Responsive Website Design With HTML / CSS Including Validations

#Delete Query 
ALTER proc [dbo].[deletehouse]
@ID nvarchar(50)
as
begin
delete from tblhouse where ID=@ID
end


#Insert Query
ALTER proc [dbo].[insertintojobtbl]
@First nvarchar(50),
@Last nvarchar(50),
@Contact nvarchar(50),
@Email nvarchar(50),
@Experience nvarchar(50),
@Qualification nvarchar(50),
@Image image,
@Date nvarchar(50)
as
begin
insert into tbljob (First, Last, Contact, Email, Experience, Qualification, Image, Date) values (@First, @Last, @Contact, @Email, @Experience, @Qualification, @Image, @Date)
end

 
#Update Query
ALTER proc [dbo].[updatepass]
@Email nvarchar(50),
@Password nvarchar(50)
as
begin
update tblregister set Password=@Password where Email=@Email
end


#Select Query
ALTER proc [dbo].[filterrent]
@Email nvarchar(50)
as
begin select * from tblrent where Email=@Email
end
 
