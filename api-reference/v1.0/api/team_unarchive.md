# <a name="unarchive-team"></a><span data-ttu-id="17dbc-101">チームを unarchive します。</span><span class="sxs-lookup"><span data-stu-id="17dbc-101">Unarchive team</span></span>



<span data-ttu-id="17dbc-102">アーカイブの[チーム](../resources/team.md)を復元します。</span><span class="sxs-lookup"><span data-stu-id="17dbc-102">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="17dbc-103">これは、メッセージを送信し、テナントとチームの設定に従いながら、チームを編集するユーザーの機能を復元します。</span><span class="sxs-lookup"><span data-stu-id="17dbc-103">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="17dbc-104">チームは、[アーカイブ](team_archive.md)の API を使用してアーカイブされます。</span><span class="sxs-lookup"><span data-stu-id="17dbc-104">Teams are archived using the [archive](team_archive.md) API.</span></span>

<span data-ttu-id="17dbc-105">Unarchiving は、非同期操作です。</span><span class="sxs-lookup"><span data-stu-id="17dbc-105">Unarchiving is an async operation.</span></span> <span data-ttu-id="17dbc-106">チームは、非同期操作が完了すると正常に、この API からの応答の後に発生する可能性がありますが、アーカイブではありません。</span><span class="sxs-lookup"><span data-stu-id="17dbc-106">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="17dbc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="17dbc-107">Permissions</span></span>
<span data-ttu-id="17dbc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17dbc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17dbc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17dbc-110">Permission type</span></span>      | <span data-ttu-id="17dbc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="17dbc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17dbc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17dbc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="17dbc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17dbc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17dbc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17dbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17dbc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17dbc-115">Not supported.</span></span>    |
|<span data-ttu-id="17dbc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17dbc-116">Application</span></span> | <span data-ttu-id="17dbc-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17dbc-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="17dbc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17dbc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="17dbc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17dbc-119">Request headers</span></span>
| <span data-ttu-id="17dbc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17dbc-120">Header</span></span>       | <span data-ttu-id="17dbc-121">値</span><span class="sxs-lookup"><span data-stu-id="17dbc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17dbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17dbc-122">Authorization</span></span>  | <span data-ttu-id="17dbc-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17dbc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17dbc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="17dbc-125">Request body</span></span>
<span data-ttu-id="17dbc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="17dbc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17dbc-127">応答</span><span class="sxs-lookup"><span data-stu-id="17dbc-127">Response</span></span>

<span data-ttu-id="17dbc-128">このメソッドを返すかどうかは、正常に起動は、unarchiving、`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="17dbc-128">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="17dbc-129">応答が含まれても、`Location`ヘッダーで、チームの unarchiving を処理するために作成された[teamsAsyncOperation](../resources/teamsasyncoperation.md)の場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17dbc-129">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="17dbc-130">この場所に GET 要求を行うことによって unarchiving の操作のステータスを確認してください。</span><span class="sxs-lookup"><span data-stu-id="17dbc-130">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="17dbc-131">例</span><span class="sxs-lookup"><span data-stu-id="17dbc-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="17dbc-132">要求</span><span class="sxs-lookup"><span data-stu-id="17dbc-132">Request</span></span>
<span data-ttu-id="17dbc-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="17dbc-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="17dbc-134">応答</span><span class="sxs-lookup"><span data-stu-id="17dbc-134">Response</span></span>
<span data-ttu-id="17dbc-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="17dbc-135">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
