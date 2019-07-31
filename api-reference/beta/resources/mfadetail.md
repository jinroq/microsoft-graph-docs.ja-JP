---
title: mfaDetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f38fae4d0360386592f956bee05d55738ad6910
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009665"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="1dd10-104">mfaDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1dd10-104">mfaDetail resource type</span></span>
<span data-ttu-id="1dd10-105">特定のサインインの MFA の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="1dd10-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="1dd10-106">これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1dd10-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="1dd10-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dd10-107">Properties</span></span>
| <span data-ttu-id="1dd10-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dd10-108">Property</span></span>     | <span data-ttu-id="1dd10-109">型</span><span class="sxs-lookup"><span data-stu-id="1dd10-109">Type</span></span>   |<span data-ttu-id="1dd10-110">説明</span><span class="sxs-lookup"><span data-stu-id="1dd10-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd10-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="1dd10-111">authDetail</span></span>|<span data-ttu-id="1dd10-112">String</span><span class="sxs-lookup"><span data-stu-id="1dd10-112">String</span></span>|<span data-ttu-id="1dd10-113">MFA が必須である、対応するサインインアクティビティの MFA 認証詳細が "Yes" であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1dd10-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="1dd10-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="1dd10-114">authMethod</span></span>|<span data-ttu-id="1dd10-115">String</span><span class="sxs-lookup"><span data-stu-id="1dd10-115">String</span></span>|<span data-ttu-id="1dd10-116">MFA 必須フィールドが "Yes" の場合に、対応するサインインアクティビティの MFA 認証方法 (SMS、Phone、Authenticator アプリ) を示します。</span><span class="sxs-lookup"><span data-stu-id="1dd10-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dd10-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1dd10-117">JSON representation</span></span>

<span data-ttu-id="1dd10-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1dd10-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
