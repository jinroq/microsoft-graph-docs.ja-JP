---
title: AppLogCollectionRequest を更新します。
description: AppLogCollectionRequest オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55974ed3c5158d4b005402fe4d6350854a197656
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430460"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="2769a-103">AppLogCollectionRequest を更新します。</span><span class="sxs-lookup"><span data-stu-id="2769a-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="2769a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2769a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2769a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2769a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2769a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2769a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2769a-107">[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2769a-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2769a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2769a-108">Prerequisites</span></span>
<span data-ttu-id="2769a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2769a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2769a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2769a-111">Permission type</span></span>|<span data-ttu-id="2769a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2769a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2769a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2769a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2769a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2769a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2769a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2769a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2769a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2769a-116">Not supported.</span></span>|
|<span data-ttu-id="2769a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2769a-117">Application</span></span>|<span data-ttu-id="2769a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2769a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2769a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2769a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="2769a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2769a-120">Request headers</span></span>
|<span data-ttu-id="2769a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2769a-121">Header</span></span>|<span data-ttu-id="2769a-122">値</span><span class="sxs-lookup"><span data-stu-id="2769a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2769a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2769a-123">Authorization</span></span>|<span data-ttu-id="2769a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2769a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2769a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2769a-125">Accept</span></span>|<span data-ttu-id="2769a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2769a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2769a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2769a-127">Request body</span></span>
<span data-ttu-id="2769a-128">要求の本文に[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2769a-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="2769a-129">[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2769a-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="2769a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2769a-130">Property</span></span>|<span data-ttu-id="2769a-131">型</span><span class="sxs-lookup"><span data-stu-id="2769a-131">Type</span></span>|<span data-ttu-id="2769a-132">説明</span><span class="sxs-lookup"><span data-stu-id="2769a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2769a-133">id</span><span class="sxs-lookup"><span data-stu-id="2769a-133">id</span></span>|<span data-ttu-id="2769a-134">String</span><span class="sxs-lookup"><span data-stu-id="2769a-134">String</span></span>|<span data-ttu-id="2769a-135">一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="2769a-135">The unique Identifier.</span></span> <span data-ttu-id="2769a-136">これは、userId_DeviceId_AppId の id です。</span><span class="sxs-lookup"><span data-stu-id="2769a-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="2769a-137">status</span><span class="sxs-lookup"><span data-stu-id="2769a-137">status</span></span>|[<span data-ttu-id="2769a-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="2769a-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="2769a-139">ログのアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="2769a-139">Log upload status.</span></span> <span data-ttu-id="2769a-140">可能な値は、`pending`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="2769a-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2769a-141">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="2769a-141">errorMessage</span></span>|<span data-ttu-id="2769a-142">String</span><span class="sxs-lookup"><span data-stu-id="2769a-142">String</span></span>|<span data-ttu-id="2769a-143">アップロード プロセス中に存在する場合のエラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="2769a-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="2769a-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="2769a-144">customLogFolders</span></span>|<span data-ttu-id="2769a-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2769a-145">String collection</span></span>|<span data-ttu-id="2769a-146">ログのフォルダーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="2769a-146">List of log folders.</span></span> |
|<span data-ttu-id="2769a-147">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="2769a-147">completedDateTime</span></span>|<span data-ttu-id="2769a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2769a-148">DateTimeOffset</span></span>|<span data-ttu-id="2769a-149">までに時間のアップロードのログ要求が終了状態</span><span class="sxs-lookup"><span data-stu-id="2769a-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="2769a-150">応答</span><span class="sxs-lookup"><span data-stu-id="2769a-150">Response</span></span>
<span data-ttu-id="2769a-151">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2769a-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2769a-152">例</span><span class="sxs-lookup"><span data-stu-id="2769a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2769a-153">要求</span><span class="sxs-lookup"><span data-stu-id="2769a-153">Request</span></span>
<span data-ttu-id="2769a-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2769a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2769a-155">応答</span><span class="sxs-lookup"><span data-stu-id="2769a-155">Response</span></span>
<span data-ttu-id="2769a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2769a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```




