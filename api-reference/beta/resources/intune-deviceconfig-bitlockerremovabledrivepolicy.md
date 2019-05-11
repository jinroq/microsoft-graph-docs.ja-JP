---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37b41d88ef73ffaf4597603e1198300f2fcdc5e1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947513"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="98a7d-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98a7d-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="98a7d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98a7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98a7d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98a7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98a7d-106">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="98a7d-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="98a7d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98a7d-107">Properties</span></span>
|<span data-ttu-id="98a7d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98a7d-108">Property</span></span>|<span data-ttu-id="98a7d-109">型</span><span class="sxs-lookup"><span data-stu-id="98a7d-109">Type</span></span>|<span data-ttu-id="98a7d-110">説明</span><span class="sxs-lookup"><span data-stu-id="98a7d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a7d-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="98a7d-111">encryptionMethod</span></span>|[<span data-ttu-id="98a7d-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="98a7d-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="98a7d-113">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="98a7d-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="98a7d-114">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="98a7d-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="98a7d-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="98a7d-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="98a7d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="98a7d-116">Boolean</span></span>|<span data-ttu-id="98a7d-117">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98a7d-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="98a7d-118">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="98a7d-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="98a7d-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="98a7d-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="98a7d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="98a7d-120">Boolean</span></span>|<span data-ttu-id="98a7d-121">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="98a7d-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98a7d-122">関係</span><span class="sxs-lookup"><span data-stu-id="98a7d-122">Relationships</span></span>
<span data-ttu-id="98a7d-123">なし</span><span class="sxs-lookup"><span data-stu-id="98a7d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98a7d-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98a7d-124">JSON Representation</span></span>
<span data-ttu-id="98a7d-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98a7d-125">Here is a JSON representation of the resource.</span></span>
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




