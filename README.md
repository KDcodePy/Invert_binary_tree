# Invert_binary_tree
Given the root of a binary tree, invert the tree, and return its root.

class TreeNode:
    def __init__(self, val=0, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right 

class Solution:
    def invert_binary(self, root: Optional[treenode]) -> Optional[treenode]:
          # if root is empty we can just return None right away
          if Not root:
              return None
          
          #initialize your left and right object
          left = self.left
          right = self.right
          
          # now we can start the swapping of the child nodes
          root.left = right 
          root.right = left 
         
          return root
