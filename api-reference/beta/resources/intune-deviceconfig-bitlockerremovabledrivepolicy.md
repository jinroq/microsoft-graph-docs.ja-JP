---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425618"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="308fb-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="308fb-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="308fb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="308fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="308fb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="308fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="308fb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="308fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="308fb-107">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="308fb-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="308fb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="308fb-108">Properties</span></span>
|<span data-ttu-id="308fb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="308fb-109">Property</span></span>|<span data-ttu-id="308fb-110">型</span><span class="sxs-lookup"><span data-stu-id="308fb-110">Type</span></span>|<span data-ttu-id="308fb-111">説明</span><span class="sxs-lookup"><span data-stu-id="308fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="308fb-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="308fb-112">encryptionMethod</span></span>|[<span data-ttu-id="308fb-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="308fb-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="308fb-114">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="308fb-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="308fb-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="308fb-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="308fb-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="308fb-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="308fb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="308fb-117">Boolean</span></span>|<span data-ttu-id="308fb-118">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="308fb-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="308fb-119">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="308fb-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="308fb-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="308fb-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="308fb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="308fb-121">Boolean</span></span>|<span data-ttu-id="308fb-122">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="308fb-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="308fb-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="308fb-123">Relationships</span></span>
<span data-ttu-id="308fb-124">なし</span><span class="sxs-lookup"><span data-stu-id="308fb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="308fb-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="308fb-125">JSON Representation</span></span>
<span data-ttu-id="308fb-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="308fb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```




