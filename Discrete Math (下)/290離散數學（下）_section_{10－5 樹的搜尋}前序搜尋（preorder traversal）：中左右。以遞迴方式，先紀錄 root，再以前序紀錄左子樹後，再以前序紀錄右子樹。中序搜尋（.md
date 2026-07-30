290
離散數學（下）

\section*{10－5 樹的搜尋}

前序搜尋（preorder traversal）：中左右。以遞迴方式，先紀錄 root，再以前序紀錄左子樹後，再以前序紀錄右子樹。
中序搜尋（inorder traversal）：左中右。以遞迴方式，先以中序紀錄左子樹，再紀錄 root，再以中序紀錄右子樹。
後序搜尋（postorder traversal）：左右中。以遞迴方式，先以後序紀錄左子樹，再以後序紀錄右子樹，再紀錄 root。

\section*{例題 1}

The inorder traversal of the following binary tree is？
【91師大資工】【91、103台大資工】
解（1）
Answer ：CBDEAFIHJG．