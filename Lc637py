class Solution(object):
    def averageOfLevels(self, root):
        result = []
        queue = [root]
        i = 0

        while i < len(queue):
            level_sum = 0
            level_count = len(queue) - i

            for _ in range(level_count):
                node = queue[i]
                i += 1

                level_sum += node.val

                if node.left:
                    queue.append(node.left)

                if node.right:
                    queue.append(node.right)

            result.append(level_sum / level_count)

        return result
