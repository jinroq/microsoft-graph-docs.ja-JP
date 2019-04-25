---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10a1039c0186238504836c0f719ab19ae4c4882
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575073"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="b0e7e-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0e7e-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="b0e7e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0e7e-105">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="b0e7e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0e7e-106">Properties</span></span>
|<span data-ttu-id="b0e7e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0e7e-107">Property</span></span>|<span data-ttu-id="b0e7e-108">型</span><span class="sxs-lookup"><span data-stu-id="b0e7e-108">Type</span></span>|<span data-ttu-id="b0e7e-109">説明</span><span class="sxs-lookup"><span data-stu-id="b0e7e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e7e-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b0e7e-110">encryptionMethod</span></span>|[<span data-ttu-id="b0e7e-111">bitlockerencryptionmethod</span><span class="sxs-lookup"><span data-stu-id="b0e7e-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="b0e7e-112">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="b0e7e-113">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="b0e7e-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b0e7e-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="b0e7e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0e7e-115">Boolean</span></span>|<span data-ttu-id="b0e7e-116">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="b0e7e-117">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="b0e7e-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b0e7e-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="b0e7e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0e7e-119">Boolean</span></span>|<span data-ttu-id="b0e7e-120">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0e7e-121">関係</span><span class="sxs-lookup"><span data-stu-id="b0e7e-121">Relationships</span></span>
<span data-ttu-id="b0e7e-122">なし</span><span class="sxs-lookup"><span data-stu-id="b0e7e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0e7e-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0e7e-123">JSON Representation</span></span>
<span data-ttu-id="b0e7e-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0e7e-124">Here is a JSON representation of the resource.</span></span>
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



