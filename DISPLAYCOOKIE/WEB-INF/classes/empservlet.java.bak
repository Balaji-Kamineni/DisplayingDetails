import javax.servlet.*;
import javax.servlet.http.*;
import java.io.*;

public class empservlet extends HttpServlet 
{
	public void service (HttpServletRequest request ,HttpServletResponse response) throws ServletException,IOException{
		response.setContentType("text/html");
		PrintWriter out=response.getWriter();
		String eno=request.getParameter("eno");
		String ename=request.getParameter("ename");
		String ecity=request.getParameter("ecity");
		Cookie ceno=new Cookie("eno",eno);
		Cookie cename=new Cookie("ename",ename);
		Cookie cecity=new Cookie("ecity",ecity);
		response.addCookie(ceno);
		response.addCookie(cename);
		response.addCookie(cecity);
		out.print("<body bgcolor=green> <form action=disp method=post>");
		out.print("<h1 align=center> Details Page <h1><hr><br>");
		out.print("<table align=center>");
		out.print("<tr> <td> Edsg </td> <td><input type=text name=edsg> </td></tr>");
		out.print("<tr> <td>Exp </td> <td> <input type=text name=exp > </td></tr>");
		out.print("<tr> <td> Sal </td> <td> <input type=text name=sal > </td></tr>");
		out.print("<tr> <td></td><td><br><input type=submit value=continue> </td></tr>");
		out.print("</table>");
		out.print("</form> </body>");
	}

}