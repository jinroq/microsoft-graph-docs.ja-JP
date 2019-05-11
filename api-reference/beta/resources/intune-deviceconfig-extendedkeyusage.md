---
title: extendedKeyUsage リソースの種類
description: カスタム拡張キー使用法の定義
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36752e9a2f86e68bd4ada1a342dc174726a684c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946953"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="646bc-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="646bc-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="646bc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="646bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="646bc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="646bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="646bc-106">カスタム拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="646bc-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="646bc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646bc-107">Properties</span></span>
|<span data-ttu-id="646bc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646bc-108">Property</span></span>|<span data-ttu-id="646bc-109">型</span><span class="sxs-lookup"><span data-stu-id="646bc-109">Type</span></span>|<span data-ttu-id="646bc-110">説明</span><span class="sxs-lookup"><span data-stu-id="646bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646bc-111">name</span><span class="sxs-lookup"><span data-stu-id="646bc-111">name</span></span>|<span data-ttu-id="646bc-112">String</span><span class="sxs-lookup"><span data-stu-id="646bc-112">String</span></span>|<span data-ttu-id="646bc-113">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="646bc-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="646bc-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="646bc-114">objectIdentifier</span></span>|<span data-ttu-id="646bc-115">String</span><span class="sxs-lookup"><span data-stu-id="646bc-115">String</span></span>|<span data-ttu-id="646bc-116">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="646bc-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="646bc-117">関係</span><span class="sxs-lookup"><span data-stu-id="646bc-117">Relationships</span></span>
<span data-ttu-id="646bc-118">なし</span><span class="sxs-lookup"><span data-stu-id="646bc-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="646bc-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="646bc-119">JSON Representation</span></span>
<span data-ttu-id="646bc-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="646bc-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




