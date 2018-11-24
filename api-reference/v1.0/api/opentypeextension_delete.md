# <a name="delete-open-extension"></a><span data-ttu-id="469d0-101">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="469d0-101">Delete open extension</span></span>

<span data-ttu-id="469d0-102">指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を削除します。</span><span class="sxs-lookup"><span data-stu-id="469d0-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="469d0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="469d0-103">Permissions</span></span>

<span data-ttu-id="469d0-104">拡張子を削除するリソース、およびアクセス許可によって委任された (アプリケーション) の種類を要求、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限の特権。</span><span class="sxs-lookup"><span data-stu-id="469d0-104">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="469d0-105">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="469d0-105">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="469d0-106">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="469d0-106">Supported resource</span></span> | <span data-ttu-id="469d0-107">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="469d0-107">Delegated (work or school account)</span></span> | <span data-ttu-id="469d0-108">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="469d0-108">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="469d0-109">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="469d0-109">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="469d0-110">デバイス</span><span class="sxs-lookup"><span data-stu-id="469d0-110">device</span></span>](../resources/device.md) | <span data-ttu-id="469d0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="469d0-111">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="469d0-112">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="469d0-112">Not supported</span></span> | <span data-ttu-id="469d0-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-113">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="469d0-114">イベント</span><span class="sxs-lookup"><span data-stu-id="469d0-114">event</span></span>](../resources/event.md) | <span data-ttu-id="469d0-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="469d0-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="469d0-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-117">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="469d0-118">グループ</span><span class="sxs-lookup"><span data-stu-id="469d0-118">group</span></span>](../resources/group.md) | <span data-ttu-id="469d0-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="469d0-120">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="469d0-120">Not supported</span></span> | <span data-ttu-id="469d0-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-121">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="469d0-122">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="469d0-122">group event</span></span>](../resources/event.md) | <span data-ttu-id="469d0-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="469d0-124">使用不可</span><span class="sxs-lookup"><span data-stu-id="469d0-124">Not supported</span></span> | <span data-ttu-id="469d0-125">使用不可</span><span class="sxs-lookup"><span data-stu-id="469d0-125">Not supported</span></span> |
| [<span data-ttu-id="469d0-126">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="469d0-126">group post</span></span>](../resources/post.md) | <span data-ttu-id="469d0-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="469d0-128">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="469d0-128">Not supported</span></span> | <span data-ttu-id="469d0-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-129">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="469d0-130">メッセージ</span><span class="sxs-lookup"><span data-stu-id="469d0-130">message</span></span>](../resources/message.md) | <span data-ttu-id="469d0-131">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-131">Mail.ReadWrite</span></span> | <span data-ttu-id="469d0-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-132">Mail.ReadWrite</span></span> | <span data-ttu-id="469d0-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-133">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="469d0-134">組織</span><span class="sxs-lookup"><span data-stu-id="469d0-134">organization</span></span>](../resources/organization.md) | <span data-ttu-id="469d0-135">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="469d0-135">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="469d0-136">使用不可</span><span class="sxs-lookup"><span data-stu-id="469d0-136">Not supported</span></span> | <span data-ttu-id="469d0-137">使用不可</span><span class="sxs-lookup"><span data-stu-id="469d0-137">Not supported</span></span> |
| [<span data-ttu-id="469d0-138">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="469d0-138">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="469d0-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-139">Contacts.ReadWrite</span></span> | <span data-ttu-id="469d0-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="469d0-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-141">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="469d0-142">ユーザー</span><span class="sxs-lookup"><span data-stu-id="469d0-142">user</span></span>](../resources/user.md) | <span data-ttu-id="469d0-143">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-143">User.ReadWrite.All</span></span> | <span data-ttu-id="469d0-144">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469d0-144">User.ReadWrite</span></span> | <span data-ttu-id="469d0-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469d0-145">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="469d0-146">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="469d0-146">HTTP request</span></span>
<span data-ttu-id="469d0-147">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。</span><span class="sxs-lookup"><span data-stu-id="469d0-147">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="469d0-p102">**注:** 上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。</span><span class="sxs-lookup"><span data-stu-id="469d0-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="469d0-150">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="469d0-150">Path parameters</span></span>
|<span data-ttu-id="469d0-151">パラメーター</span><span class="sxs-lookup"><span data-stu-id="469d0-151">Parameter</span></span>|<span data-ttu-id="469d0-152">型</span><span class="sxs-lookup"><span data-stu-id="469d0-152">Type</span></span>|<span data-ttu-id="469d0-153">説明</span><span class="sxs-lookup"><span data-stu-id="469d0-153">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="469d0-154">ID</span><span class="sxs-lookup"><span data-stu-id="469d0-154">id</span></span>|<span data-ttu-id="469d0-155">文字列</span><span class="sxs-lookup"><span data-stu-id="469d0-155">string</span></span>|<span data-ttu-id="469d0-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="469d0-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="469d0-158">extensionId</span><span class="sxs-lookup"><span data-stu-id="469d0-158">extensionId</span></span>|<span data-ttu-id="469d0-159">文字列</span><span class="sxs-lookup"><span data-stu-id="469d0-159">string</span></span>|<span data-ttu-id="469d0-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="469d0-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="469d0-163">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="469d0-163">Request headers</span></span>
| <span data-ttu-id="469d0-164">名前</span><span class="sxs-lookup"><span data-stu-id="469d0-164">Name</span></span>       | <span data-ttu-id="469d0-165">値</span><span class="sxs-lookup"><span data-stu-id="469d0-165">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="469d0-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="469d0-166">Authorization</span></span> | <span data-ttu-id="469d0-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="469d0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="469d0-169">要求本文</span><span class="sxs-lookup"><span data-stu-id="469d0-169">Request body</span></span>
<span data-ttu-id="469d0-170">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="469d0-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="469d0-171">応答</span><span class="sxs-lookup"><span data-stu-id="469d0-171">Response</span></span>

<span data-ttu-id="469d0-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="469d0-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="469d0-174">例</span><span class="sxs-lookup"><span data-stu-id="469d0-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="469d0-175">要求</span><span class="sxs-lookup"><span data-stu-id="469d0-175">Request</span></span>
<span data-ttu-id="469d0-176">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="469d0-176">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="469d0-177">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="469d0-177">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="469d0-178">応答</span><span class="sxs-lookup"><span data-stu-id="469d0-178">Response</span></span>
<span data-ttu-id="469d0-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="469d0-179">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->