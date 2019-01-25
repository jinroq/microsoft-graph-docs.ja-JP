---
title: publicClient リソースの種類
description: 以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525963"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="6d44c-104">publicClient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d44c-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d44c-105">以外の Web アプリケーションまたは Web Api の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d44c-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="6d44c-106">(モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)</span><span class="sxs-lookup"><span data-stu-id="6d44c-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="6d44c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d44c-107">Properties</span></span>

| <span data-ttu-id="6d44c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d44c-108">Property</span></span> | <span data-ttu-id="6d44c-109">型</span><span class="sxs-lookup"><span data-stu-id="6d44c-109">Type</span></span> | <span data-ttu-id="6d44c-110">説明</span><span class="sxs-lookup"><span data-stu-id="6d44c-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6d44c-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="6d44c-111">redirectUris</span></span>|<span data-ttu-id="6d44c-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6d44c-112">String collection</span></span>| <span data-ttu-id="6d44c-113">ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d44c-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d44c-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d44c-114">JSON representation</span></span>
<span data-ttu-id="6d44c-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6d44c-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
