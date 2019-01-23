---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399935"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="1d946-103">windowsEnrollmentStatusScreenSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d946-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="1d946-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d946-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d946-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d946-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d946-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d946-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d946-107">登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="1d946-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="1d946-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d946-108">Properties</span></span>
|<span data-ttu-id="1d946-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d946-109">Property</span></span>|<span data-ttu-id="1d946-110">型</span><span class="sxs-lookup"><span data-stu-id="1d946-110">Type</span></span>|<span data-ttu-id="1d946-111">説明</span><span class="sxs-lookup"><span data-stu-id="1d946-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d946-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="1d946-112">hideInstallationProgress</span></span>|<span data-ttu-id="1d946-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d946-113">Boolean</span></span>|<span data-ttu-id="1d946-114">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="1d946-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="1d946-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="1d946-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="1d946-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d946-116">Boolean</span></span>|<span data-ttu-id="1d946-117">許可またはブロックのユーザー プロファイル、およびアプリケーション インストールが完了する前にデバイスを使用するには</span><span class="sxs-lookup"><span data-stu-id="1d946-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="1d946-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="1d946-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="1d946-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d946-119">Boolean</span></span>|<span data-ttu-id="1d946-120">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="1d946-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="1d946-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="1d946-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="1d946-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d946-122">Boolean</span></span>|<span data-ttu-id="1d946-123">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="1d946-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="1d946-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="1d946-124">customErrorMessage</span></span>|<span data-ttu-id="1d946-125">String</span><span class="sxs-lookup"><span data-stu-id="1d946-125">String</span></span>|<span data-ttu-id="1d946-126">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="1d946-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="1d946-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d946-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="1d946-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1d946-128">Int32</span></span>|<span data-ttu-id="1d946-129">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="1d946-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="1d946-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="1d946-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="1d946-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d946-131">Boolean</span></span>|<span data-ttu-id="1d946-132">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="1d946-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d946-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d946-133">Relationships</span></span>
<span data-ttu-id="1d946-134">なし</span><span class="sxs-lookup"><span data-stu-id="1d946-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d946-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d946-135">JSON Representation</span></span>
<span data-ttu-id="1d946-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d946-136">Here is a JSON representation of the resource.</span></span>
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




