<span data-ttu-id="1a864-p105">次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。</span><span class="sxs-lookup"><span data-stu-id="1a864-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。

| <span data-ttu-id="1a864-162">名前</span><span class="sxs-lookup"><span data-stu-id="1a864-162">Name</span></span>           | <span data-ttu-id="1a864-163">解像度</span><span class="sxs-lookup"><span data-stu-id="1a864-163">Resolution</span></span>  | <span data-ttu-id="1a864-164">縦横比</span><span class="sxs-lookup"><span data-stu-id="1a864-164">Aspect Ratio</span></span> | <span data-ttu-id="1a864-165">説明</span><span class="sxs-lookup"><span data-stu-id="1a864-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="1a864-166">96 longest</span><span class="sxs-lookup"><span data-stu-id="1a864-166">96 longest</span></span>  | <span data-ttu-id="1a864-167">Original</span><span class="sxs-lookup"><span data-stu-id="1a864-167">Original</span></span>     | <span data-ttu-id="1a864-168">圧縮率の高い小さなサムネイルは、正方形にトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="1a864-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="1a864-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="1a864-169">176 longest</span></span> | <span data-ttu-id="1a864-170">Original</span><span class="sxs-lookup"><span data-stu-id="1a864-170">Original</span></span>     | <span data-ttu-id="1a864-171">OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="1a864-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="1a864-172">800 longest</span><span class="sxs-lookup"><span data-stu-id="1a864-172">800 longest</span></span> | <span data-ttu-id="1a864-173">Original</span><span class="sxs-lookup"><span data-stu-id="1a864-173">Original</span></span>     | <span data-ttu-id="1a864-174">サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。</span><span class="sxs-lookup"><span data-stu-id="1a864-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <span data-ttu-id="1a864-175">注釈</span><span class="sxs-lookup"><span data-stu-id="1a864-175">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="1a864-176">**注:** OneDrive for Business および SharePoint の場合:</span><span class="sxs-lookup"><span data-stu-id="1a864-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="1a864-177">次の呼び出しを使用したサムネイル コレクションの展開は機能しません: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="1a864-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
