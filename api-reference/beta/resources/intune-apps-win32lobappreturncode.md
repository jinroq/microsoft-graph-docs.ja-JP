---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリのリターンコードプロパティを格納します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c05d695b05a001e6854e254bf065d6fb41ba773
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461088"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="28b61-103">win32LobAppReturnCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28b61-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="28b61-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28b61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28b61-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28b61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28b61-106">Win32 アプリのリターンコードプロパティを格納します。</span><span class="sxs-lookup"><span data-stu-id="28b61-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="28b61-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28b61-107">Properties</span></span>
|<span data-ttu-id="28b61-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28b61-108">Property</span></span>|<span data-ttu-id="28b61-109">型</span><span class="sxs-lookup"><span data-stu-id="28b61-109">Type</span></span>|<span data-ttu-id="28b61-110">説明</span><span class="sxs-lookup"><span data-stu-id="28b61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b61-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="28b61-111">returnCode</span></span>|<span data-ttu-id="28b61-112">Int32</span><span class="sxs-lookup"><span data-stu-id="28b61-112">Int32</span></span>|<span data-ttu-id="28b61-113">コードを返します。</span><span class="sxs-lookup"><span data-stu-id="28b61-113">Return code.</span></span>|
|<span data-ttu-id="28b61-114">type</span><span class="sxs-lookup"><span data-stu-id="28b61-114">type</span></span>|[<span data-ttu-id="28b61-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="28b61-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="28b61-116">戻り値のコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="28b61-116">The type of return code.</span></span> <span data-ttu-id="28b61-117">可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。</span><span class="sxs-lookup"><span data-stu-id="28b61-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b61-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28b61-118">Relationships</span></span>
<span data-ttu-id="28b61-119">なし</span><span class="sxs-lookup"><span data-stu-id="28b61-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28b61-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28b61-120">JSON Representation</span></span>
<span data-ttu-id="28b61-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28b61-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





