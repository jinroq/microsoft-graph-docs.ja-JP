---
title: publicclientapplication リソースの種類
description: 非 web アプリまたは web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)
localization_priority: Normal
ms.openlocfilehash: 8118d1e771cb55ce5b82c9ddac14aaa45260ab56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348869"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="cc42d-104">publicclientapplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc42d-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc42d-105">非 web アプリまたは web Api の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc42d-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="cc42d-106">(たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)</span><span class="sxs-lookup"><span data-stu-id="cc42d-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="cc42d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc42d-107">Properties</span></span>

| <span data-ttu-id="cc42d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc42d-108">Property</span></span> | <span data-ttu-id="cc42d-109">型</span><span class="sxs-lookup"><span data-stu-id="cc42d-109">Type</span></span> | <span data-ttu-id="cc42d-110">説明</span><span class="sxs-lookup"><span data-stu-id="cc42d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cc42d-111">redirecturis</span><span class="sxs-lookup"><span data-stu-id="cc42d-111">redirectUris</span></span>|<span data-ttu-id="cc42d-112">String collection</span><span class="sxs-lookup"><span data-stu-id="cc42d-112">String collection</span></span>| <span data-ttu-id="cc42d-113">サインインのためにユーザートークンが送信される url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト uri を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc42d-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc42d-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc42d-114">JSON representation</span></span>
<span data-ttu-id="cc42d-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc42d-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
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
  "suppressions": []
}
-->
