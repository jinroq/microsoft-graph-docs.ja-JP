---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリのインストール環境のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c981c2ae9842e928d35ec05f146955dd766d6c35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012297"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="ad13c-103">win32LobAppInstallExperience リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad13c-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="ad13c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad13c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad13c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad13c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad13c-106">Win32 アプリのインストール環境のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ad13c-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="ad13c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad13c-107">Properties</span></span>
|<span data-ttu-id="ad13c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad13c-108">Property</span></span>|<span data-ttu-id="ad13c-109">型</span><span class="sxs-lookup"><span data-stu-id="ad13c-109">Type</span></span>|<span data-ttu-id="ad13c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad13c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad13c-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="ad13c-111">runAsAccount</span></span>|[<span data-ttu-id="ad13c-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="ad13c-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="ad13c-113">アプリが実行されている実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ad13c-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="ad13c-114">可能な値: `system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="ad13c-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad13c-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad13c-115">Relationships</span></span>
<span data-ttu-id="ad13c-116">なし</span><span class="sxs-lookup"><span data-stu-id="ad13c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad13c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad13c-117">JSON Representation</span></span>
<span data-ttu-id="ad13c-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad13c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





