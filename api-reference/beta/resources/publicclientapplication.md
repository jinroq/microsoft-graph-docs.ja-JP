---
title: publicClientApplication リソースの種類
description: 非 Web アプリまたは Web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4503e65777b41fc2f864cd818697b048e3c8e435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965559"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="d087a-104">publicClientApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d087a-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d087a-105">非 Web アプリまたは Web Api の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="d087a-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="d087a-106">(たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)</span><span class="sxs-lookup"><span data-stu-id="d087a-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="d087a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d087a-107">Properties</span></span>

| <span data-ttu-id="d087a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d087a-108">Property</span></span> | <span data-ttu-id="d087a-109">型</span><span class="sxs-lookup"><span data-stu-id="d087a-109">Type</span></span> | <span data-ttu-id="d087a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d087a-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d087a-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="d087a-111">redirectUris</span></span>|<span data-ttu-id="d087a-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d087a-112">String collection</span></span>| <span data-ttu-id="d087a-113">サインインのためにユーザートークンが送信される Url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト Uri を指定します。</span><span class="sxs-lookup"><span data-stu-id="d087a-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d087a-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d087a-114">JSON representation</span></span>
<span data-ttu-id="d087a-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d087a-115">Here is a JSON representation of the resource.</span></span>

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
