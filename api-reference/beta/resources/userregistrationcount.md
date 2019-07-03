---
title: userRegistrationCount リソースの種類
description: テナント内のユーザーの登録数と状態を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 43f151864f7ca996602e7bd2fc42f3fa4ba743d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487165"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="904ad-103">userRegistrationCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="904ad-103">userRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="904ad-104">テナント内のユーザーの登録数と状態を表します。</span><span class="sxs-lookup"><span data-stu-id="904ad-104">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="904ad-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="904ad-105">Properties</span></span>

| <span data-ttu-id="904ad-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="904ad-106">Property</span></span>     | <span data-ttu-id="904ad-107">型</span><span class="sxs-lookup"><span data-stu-id="904ad-107">Type</span></span>        | <span data-ttu-id="904ad-108">説明</span><span class="sxs-lookup"><span data-stu-id="904ad-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="904ad-109">registrationCount</span><span class="sxs-lookup"><span data-stu-id="904ad-109">registrationCount</span></span> | <span data-ttu-id="904ad-110">Int64</span><span class="sxs-lookup"><span data-stu-id="904ad-110">Int64</span></span> | <span data-ttu-id="904ad-111">テナントの登録数を示します。</span><span class="sxs-lookup"><span data-stu-id="904ad-111">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="904ad-112">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="904ad-112">registrationStatus</span></span> | <span data-ttu-id="904ad-113">String</span><span class="sxs-lookup"><span data-stu-id="904ad-113">String</span></span> | <span data-ttu-id="904ad-114">ユーザー登録の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="904ad-114">Represents the status of user registration.</span></span> <span data-ttu-id="904ad-115">可能な値は`registered`、 `enabled`、 `capable`、、 `mfaRegistered`です。</span><span class="sxs-lookup"><span data-stu-id="904ad-115">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="904ad-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="904ad-116">JSON representation</span></span>

<span data-ttu-id="904ad-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="904ad-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->