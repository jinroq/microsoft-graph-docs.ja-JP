---
title: AppLogCollectionRequest を作成します。
description: 新しい appLogCollectionRequest オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c3afd1cf00ba706e3fbc1e960e649fc010ae582f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430446"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="33987-103">AppLogCollectionRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="33987-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="33987-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33987-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33987-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33987-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33987-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33987-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33987-107">新しい[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="33987-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33987-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="33987-108">Prerequisites</span></span>
<span data-ttu-id="33987-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33987-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33987-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33987-111">Permission type</span></span>|<span data-ttu-id="33987-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33987-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33987-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33987-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33987-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33987-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="33987-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33987-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33987-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33987-116">Not supported.</span></span>|
|<span data-ttu-id="33987-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33987-117">Application</span></span>|<span data-ttu-id="33987-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33987-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33987-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33987-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="33987-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33987-120">Request headers</span></span>
|<span data-ttu-id="33987-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33987-121">Header</span></span>|<span data-ttu-id="33987-122">値</span><span class="sxs-lookup"><span data-stu-id="33987-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33987-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33987-123">Authorization</span></span>|<span data-ttu-id="33987-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="33987-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33987-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33987-125">Accept</span></span>|<span data-ttu-id="33987-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33987-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33987-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="33987-127">Request body</span></span>
<span data-ttu-id="33987-128">要求の本文に appLogCollectionRequest オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="33987-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="33987-129">次の表は、appLogCollectionRequest を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="33987-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="33987-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33987-130">Property</span></span>|<span data-ttu-id="33987-131">型</span><span class="sxs-lookup"><span data-stu-id="33987-131">Type</span></span>|<span data-ttu-id="33987-132">説明</span><span class="sxs-lookup"><span data-stu-id="33987-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33987-133">id</span><span class="sxs-lookup"><span data-stu-id="33987-133">id</span></span>|<span data-ttu-id="33987-134">String</span><span class="sxs-lookup"><span data-stu-id="33987-134">String</span></span>|<span data-ttu-id="33987-135">一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="33987-135">The unique Identifier.</span></span> <span data-ttu-id="33987-136">これは、userId_DeviceId_AppId の id です。</span><span class="sxs-lookup"><span data-stu-id="33987-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="33987-137">status</span><span class="sxs-lookup"><span data-stu-id="33987-137">status</span></span>|[<span data-ttu-id="33987-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="33987-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="33987-139">ログのアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="33987-139">Log upload status.</span></span> <span data-ttu-id="33987-140">可能な値は、`pending`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="33987-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="33987-141">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="33987-141">errorMessage</span></span>|<span data-ttu-id="33987-142">String</span><span class="sxs-lookup"><span data-stu-id="33987-142">String</span></span>|<span data-ttu-id="33987-143">アップロード プロセス中に存在する場合のエラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="33987-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="33987-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="33987-144">customLogFolders</span></span>|<span data-ttu-id="33987-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="33987-145">String collection</span></span>|<span data-ttu-id="33987-146">ログのフォルダーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="33987-146">List of log folders.</span></span> |
|<span data-ttu-id="33987-147">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="33987-147">completedDateTime</span></span>|<span data-ttu-id="33987-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33987-148">DateTimeOffset</span></span>|<span data-ttu-id="33987-149">までに時間のアップロードのログ要求が終了状態</span><span class="sxs-lookup"><span data-stu-id="33987-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="33987-150">応答</span><span class="sxs-lookup"><span data-stu-id="33987-150">Response</span></span>
<span data-ttu-id="33987-151">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="33987-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33987-152">例</span><span class="sxs-lookup"><span data-stu-id="33987-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="33987-153">要求</span><span class="sxs-lookup"><span data-stu-id="33987-153">Request</span></span>
<span data-ttu-id="33987-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33987-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
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

### <a name="response"></a><span data-ttu-id="33987-155">応答</span><span class="sxs-lookup"><span data-stu-id="33987-155">Response</span></span>
<span data-ttu-id="33987-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33987-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




