---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 297296dae82a172f68b04ca13eeb9200a33aaba0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964208"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="d2b74-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="d2b74-103">Create managedAppOperation</span></span>

> <span data-ttu-id="d2b74-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2b74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2b74-105">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2b74-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2b74-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2b74-106">Prerequisites</span></span>
<span data-ttu-id="d2b74-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2b74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2b74-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2b74-109">Permission type</span></span>|<span data-ttu-id="d2b74-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2b74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2b74-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2b74-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2b74-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2b74-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2b74-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2b74-114">Not supported.</span></span>|
|<span data-ttu-id="d2b74-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2b74-115">Application</span></span>|<span data-ttu-id="d2b74-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2b74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2b74-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2b74-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="d2b74-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b74-118">Request headers</span></span>
|<span data-ttu-id="d2b74-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b74-119">Header</span></span>|<span data-ttu-id="d2b74-120">値</span><span class="sxs-lookup"><span data-stu-id="d2b74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2b74-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b74-121">Authorization</span></span>|<span data-ttu-id="d2b74-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d2b74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2b74-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d2b74-123">Accept</span></span>|<span data-ttu-id="d2b74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d2b74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2b74-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2b74-125">Request body</span></span>
<span data-ttu-id="d2b74-126">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2b74-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="d2b74-127">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2b74-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="d2b74-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2b74-128">Property</span></span>|<span data-ttu-id="d2b74-129">型</span><span class="sxs-lookup"><span data-stu-id="d2b74-129">Type</span></span>|<span data-ttu-id="d2b74-130">説明</span><span class="sxs-lookup"><span data-stu-id="d2b74-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2b74-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d2b74-131">displayName</span></span>|<span data-ttu-id="d2b74-132">String</span><span class="sxs-lookup"><span data-stu-id="d2b74-132">String</span></span>|<span data-ttu-id="d2b74-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="d2b74-133">The operation name.</span></span>|
|<span data-ttu-id="d2b74-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2b74-134">lastModifiedDateTime</span></span>|<span data-ttu-id="d2b74-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2b74-135">DateTimeOffset</span></span>|<span data-ttu-id="d2b74-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="d2b74-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="d2b74-137">state</span><span class="sxs-lookup"><span data-stu-id="d2b74-137">state</span></span>|<span data-ttu-id="d2b74-138">String</span><span class="sxs-lookup"><span data-stu-id="d2b74-138">String</span></span>|<span data-ttu-id="d2b74-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="d2b74-139">The current state of the operation</span></span>|
|<span data-ttu-id="d2b74-140">id</span><span class="sxs-lookup"><span data-stu-id="d2b74-140">id</span></span>|<span data-ttu-id="d2b74-141">String</span><span class="sxs-lookup"><span data-stu-id="d2b74-141">String</span></span>|<span data-ttu-id="d2b74-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2b74-142">Key of the entity.</span></span>|
|<span data-ttu-id="d2b74-143">version</span><span class="sxs-lookup"><span data-stu-id="d2b74-143">version</span></span>|<span data-ttu-id="d2b74-144">String</span><span class="sxs-lookup"><span data-stu-id="d2b74-144">String</span></span>|<span data-ttu-id="d2b74-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d2b74-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d2b74-146">応答</span><span class="sxs-lookup"><span data-stu-id="d2b74-146">Response</span></span>
<span data-ttu-id="d2b74-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2b74-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b74-148">例</span><span class="sxs-lookup"><span data-stu-id="d2b74-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2b74-149">要求</span><span class="sxs-lookup"><span data-stu-id="d2b74-149">Request</span></span>
<span data-ttu-id="d2b74-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2b74-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="d2b74-151">応答</span><span class="sxs-lookup"><span data-stu-id="d2b74-151">Response</span></span>
<span data-ttu-id="d2b74-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2b74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



