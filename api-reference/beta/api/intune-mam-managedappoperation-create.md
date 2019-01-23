---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4ffc03237e034321dab2bf2a03bdcca0cfbe505c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399060"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="45470-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="45470-103">Create managedAppOperation</span></span>

> <span data-ttu-id="45470-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="45470-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45470-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45470-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45470-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45470-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45470-107">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45470-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45470-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="45470-108">Prerequisites</span></span>
<span data-ttu-id="45470-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45470-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45470-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45470-111">Permission type</span></span>|<span data-ttu-id="45470-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45470-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45470-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45470-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45470-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45470-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45470-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45470-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45470-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45470-116">Not supported.</span></span>|
|<span data-ttu-id="45470-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45470-117">Application</span></span>|<span data-ttu-id="45470-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45470-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45470-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45470-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="45470-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45470-120">Request headers</span></span>
|<span data-ttu-id="45470-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45470-121">Header</span></span>|<span data-ttu-id="45470-122">値</span><span class="sxs-lookup"><span data-stu-id="45470-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45470-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45470-123">Authorization</span></span>|<span data-ttu-id="45470-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="45470-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45470-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45470-125">Accept</span></span>|<span data-ttu-id="45470-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45470-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45470-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="45470-127">Request body</span></span>
<span data-ttu-id="45470-128">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45470-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="45470-129">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45470-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="45470-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45470-130">Property</span></span>|<span data-ttu-id="45470-131">型</span><span class="sxs-lookup"><span data-stu-id="45470-131">Type</span></span>|<span data-ttu-id="45470-132">説明</span><span class="sxs-lookup"><span data-stu-id="45470-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45470-133">displayName</span><span class="sxs-lookup"><span data-stu-id="45470-133">displayName</span></span>|<span data-ttu-id="45470-134">String</span><span class="sxs-lookup"><span data-stu-id="45470-134">String</span></span>|<span data-ttu-id="45470-135">操作名。</span><span class="sxs-lookup"><span data-stu-id="45470-135">The operation name.</span></span>|
|<span data-ttu-id="45470-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45470-136">lastModifiedDateTime</span></span>|<span data-ttu-id="45470-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45470-137">DateTimeOffset</span></span>|<span data-ttu-id="45470-138">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="45470-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="45470-139">state</span><span class="sxs-lookup"><span data-stu-id="45470-139">state</span></span>|<span data-ttu-id="45470-140">String</span><span class="sxs-lookup"><span data-stu-id="45470-140">String</span></span>|<span data-ttu-id="45470-141">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="45470-141">The current state of the operation</span></span>|
|<span data-ttu-id="45470-142">id</span><span class="sxs-lookup"><span data-stu-id="45470-142">id</span></span>|<span data-ttu-id="45470-143">String</span><span class="sxs-lookup"><span data-stu-id="45470-143">String</span></span>|<span data-ttu-id="45470-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45470-144">Key of the entity.</span></span>|
|<span data-ttu-id="45470-145">version</span><span class="sxs-lookup"><span data-stu-id="45470-145">version</span></span>|<span data-ttu-id="45470-146">String</span><span class="sxs-lookup"><span data-stu-id="45470-146">String</span></span>|<span data-ttu-id="45470-147">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="45470-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="45470-148">応答</span><span class="sxs-lookup"><span data-stu-id="45470-148">Response</span></span>
<span data-ttu-id="45470-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45470-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45470-150">例</span><span class="sxs-lookup"><span data-stu-id="45470-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="45470-151">要求</span><span class="sxs-lookup"><span data-stu-id="45470-151">Request</span></span>
<span data-ttu-id="45470-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45470-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="45470-153">応答</span><span class="sxs-lookup"><span data-stu-id="45470-153">Response</span></span>
<span data-ttu-id="45470-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45470-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```




