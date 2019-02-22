---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録の状態画面の設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684a447b82f285784eda1bf71c13f35d766a570
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148686"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="1bd2e-103">windowsEnrollmentStatusScreenSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bd2e-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="1bd2e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bd2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd2e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1bd2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd2e-106">登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="1bd2e-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="1bd2e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bd2e-107">Properties</span></span>
|<span data-ttu-id="1bd2e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bd2e-108">Property</span></span>|<span data-ttu-id="1bd2e-109">型</span><span class="sxs-lookup"><span data-stu-id="1bd2e-109">Type</span></span>|<span data-ttu-id="1bd2e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1bd2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd2e-111">hideinstallationprogress 進行状況</span><span class="sxs-lookup"><span data-stu-id="1bd2e-111">hideInstallationProgress</span></span>|<span data-ttu-id="1bd2e-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="1bd2e-112">Boolean</span></span>|<span data-ttu-id="1bd2e-113">ユーザーにインストールの進行状況を表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="1bd2e-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="1bd2e-114">allowdeviceusebeforeprofileandappinstallcomplete</span><span class="sxs-lookup"><span data-stu-id="1bd2e-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="1bd2e-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="1bd2e-115">Boolean</span></span>|<span data-ttu-id="1bd2e-116">プロファイルとアプリのインストールが完了する前にユーザーがデバイスを使用することを許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="1bd2e-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="1bd2e-117">blockdevicesetupretrybyuser</span><span class="sxs-lookup"><span data-stu-id="1bd2e-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="1bd2e-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="1bd2e-118">Boolean</span></span>|<span data-ttu-id="1bd2e-119">ユーザーがインストールエラー時にセットアップを再試行できるようにする</span><span class="sxs-lookup"><span data-stu-id="1bd2e-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="1bd2e-120">allowlogcollectiononinstallfailure</span><span class="sxs-lookup"><span data-stu-id="1bd2e-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="1bd2e-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="1bd2e-121">Boolean</span></span>|<span data-ttu-id="1bd2e-122">インストール失敗時にログ収集を許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="1bd2e-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="1bd2e-123">customerrormessage</span><span class="sxs-lookup"><span data-stu-id="1bd2e-123">customErrorMessage</span></span>|<span data-ttu-id="1bd2e-124">String</span><span class="sxs-lookup"><span data-stu-id="1bd2e-124">String</span></span>|<span data-ttu-id="1bd2e-125">インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する</span><span class="sxs-lookup"><span data-stu-id="1bd2e-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="1bd2e-126">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1bd2e-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="1bd2e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1bd2e-127">Int32</span></span>|<span data-ttu-id="1bd2e-128">インストールの進行状況のタイムアウトを分単位で設定する</span><span class="sxs-lookup"><span data-stu-id="1bd2e-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="1bd2e-129">allowdeviceuseoninstallfailure</span><span class="sxs-lookup"><span data-stu-id="1bd2e-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="1bd2e-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="1bd2e-130">Boolean</span></span>|<span data-ttu-id="1bd2e-131">インストールエラー時にユーザーがデバイスを引き続き使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="1bd2e-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bd2e-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1bd2e-132">Relationships</span></span>
<span data-ttu-id="1bd2e-133">なし</span><span class="sxs-lookup"><span data-stu-id="1bd2e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bd2e-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1bd2e-134">JSON Representation</span></span>
<span data-ttu-id="1bd2e-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1bd2e-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```




