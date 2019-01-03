---
title: チームを unarchive します。
description: アーカイブされたチームを復元します。 これは、メッセージを送信し、テナントとチームの設定に従いながら、チームを編集するユーザーの機能を復元します。 チームは、アーカイブの API を使用してアーカイブされます。
ms.openlocfilehash: 7507a58ef75939110d0c740e20d8540838bda204
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222612"
---
# <a name="unarchive-team"></a><span data-ttu-id="412b1-105">チームを unarchive します。</span><span class="sxs-lookup"><span data-stu-id="412b1-105">Unarchive team</span></span>



<span data-ttu-id="412b1-106">アーカイブの[チーム](../resources/team.md)を復元します。</span><span class="sxs-lookup"><span data-stu-id="412b1-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="412b1-107">これは、メッセージを送信し、テナントとチームの設定に従いながら、チームを編集するユーザーの機能を復元します。</span><span class="sxs-lookup"><span data-stu-id="412b1-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="412b1-108">チームは、[アーカイブ](team-archive.md)の API を使用してアーカイブされます。</span><span class="sxs-lookup"><span data-stu-id="412b1-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="412b1-109">Unarchiving は、非同期操作です。</span><span class="sxs-lookup"><span data-stu-id="412b1-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="412b1-110">チームは、非同期操作が完了すると正常に、この API からの応答の後に発生する可能性がありますが、アーカイブではありません。</span><span class="sxs-lookup"><span data-stu-id="412b1-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="412b1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="412b1-111">Permissions</span></span>
<span data-ttu-id="412b1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="412b1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412b1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="412b1-114">Permission type</span></span>      | <span data-ttu-id="412b1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="412b1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="412b1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="412b1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="412b1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="412b1-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="412b1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="412b1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="412b1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="412b1-119">Not supported.</span></span>    |
|<span data-ttu-id="412b1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="412b1-120">Application</span></span> | <span data-ttu-id="412b1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="412b1-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="412b1-122">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="412b1-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="412b1-123">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="412b1-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="412b1-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="412b1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="412b1-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="412b1-125">Request headers</span></span>
| <span data-ttu-id="412b1-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="412b1-126">Header</span></span>       | <span data-ttu-id="412b1-127">値</span><span class="sxs-lookup"><span data-stu-id="412b1-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="412b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="412b1-128">Authorization</span></span>  | <span data-ttu-id="412b1-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="412b1-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="412b1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="412b1-131">Request body</span></span>
<span data-ttu-id="412b1-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="412b1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="412b1-133">応答</span><span class="sxs-lookup"><span data-stu-id="412b1-133">Response</span></span>

<span data-ttu-id="412b1-134">このメソッドを返すかどうかは、正常に起動は、unarchiving、`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="412b1-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="412b1-135">応答が含まれても、`Location`ヘッダーで、チームの unarchiving を処理するために作成された[teamsAsyncOperation](../resources/teamsasyncoperation.md)の場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="412b1-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="412b1-136">この場所に GET 要求を行うことによって unarchiving の操作のステータスを確認してください。</span><span class="sxs-lookup"><span data-stu-id="412b1-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="412b1-137">例</span><span class="sxs-lookup"><span data-stu-id="412b1-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="412b1-138">要求</span><span class="sxs-lookup"><span data-stu-id="412b1-138">Request</span></span>
<span data-ttu-id="412b1-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="412b1-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="412b1-140">応答</span><span class="sxs-lookup"><span data-stu-id="412b1-140">Response</span></span>
<span data-ttu-id="412b1-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="412b1-141">The following is an example of a response.</span></span>
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