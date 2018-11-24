# <a name="add-tab-to-channel"></a><span data-ttu-id="725a1-101">チャネルにタブを追加します。</span><span class="sxs-lookup"><span data-stu-id="725a1-101">Add tab to channel</span></span>



<span data-ttu-id="725a1-102">(ピン) を追加する[チーム](../resources/team.md)内で指定された[チャネル](../resources/channel.md)を[タブ](../resources/teamstab.md)します。</span><span class="sxs-lookup"><span data-stu-id="725a1-102">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="725a1-103">対応するアプリケーションでは、[チームにインストールされている](../api/teamsappinstallation_add.md)ある必要があります。</span><span class="sxs-lookup"><span data-stu-id="725a1-103">The corresponding app must already be [installed in the team](../api/teamsappinstallation_add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="725a1-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="725a1-104">Permissions</span></span>
<span data-ttu-id="725a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="725a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="725a1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="725a1-107">Permission type</span></span>      | <span data-ttu-id="725a1-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="725a1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="725a1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="725a1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="725a1-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725a1-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="725a1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="725a1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="725a1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="725a1-112">Not supported.</span></span>    |
| <span data-ttu-id="725a1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="725a1-113">Application</span></span>                            | <span data-ttu-id="725a1-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725a1-114">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="725a1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="725a1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="725a1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="725a1-116">Request headers</span></span>
| <span data-ttu-id="725a1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="725a1-117">Header</span></span>       | <span data-ttu-id="725a1-118">値</span><span class="sxs-lookup"><span data-stu-id="725a1-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="725a1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="725a1-119">Authorization</span></span>  | <span data-ttu-id="725a1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="725a1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="725a1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="725a1-122">Request body</span></span>

<span data-ttu-id="725a1-123">[TeamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="725a1-123">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="725a1-124">応答</span><span class="sxs-lookup"><span data-stu-id="725a1-124">Response</span></span>

<span data-ttu-id="725a1-125">成功した場合、このメソッドは `201 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="725a1-125">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="725a1-126">例</span><span class="sxs-lookup"><span data-stu-id="725a1-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="725a1-127">要求</span><span class="sxs-lookup"><span data-stu-id="725a1-127">Request</span></span>

<span data-ttu-id="725a1-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="725a1-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="725a1-129">応答</span><span class="sxs-lookup"><span data-stu-id="725a1-129">Response</span></span>

<span data-ttu-id="725a1-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="725a1-130">The following is an example of the response.</span></span> <span data-ttu-id="725a1-131">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="725a1-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="725a1-132">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="725a1-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "name": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="725a1-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="725a1-133">See also</span></span>

[<span data-ttu-id="725a1-134">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="725a1-134">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
