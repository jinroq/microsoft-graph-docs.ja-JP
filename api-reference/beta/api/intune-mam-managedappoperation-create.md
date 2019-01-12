---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a8be6117a14a2ce87d06928ec8f45fde87c52d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979867"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="2ef57-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="2ef57-103">Create managedAppOperation</span></span>

> <span data-ttu-id="2ef57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ef57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ef57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ef57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ef57-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ef57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ef57-107">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2ef57-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ef57-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ef57-108">Prerequisites</span></span>
<span data-ttu-id="2ef57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ef57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef57-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ef57-111">Permission type</span></span>|<span data-ttu-id="2ef57-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ef57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ef57-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ef57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ef57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ef57-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ef57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ef57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ef57-116">Not supported.</span></span>|
|<span data-ttu-id="2ef57-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ef57-117">Application</span></span>|<span data-ttu-id="2ef57-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ef57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ef57-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ef57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="2ef57-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ef57-120">Request headers</span></span>
|<span data-ttu-id="2ef57-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ef57-121">Header</span></span>|<span data-ttu-id="2ef57-122">値</span><span class="sxs-lookup"><span data-stu-id="2ef57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ef57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef57-123">Authorization</span></span>|<span data-ttu-id="2ef57-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2ef57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ef57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ef57-125">Accept</span></span>|<span data-ttu-id="2ef57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ef57-127">Request body</span></span>
<span data-ttu-id="2ef57-128">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ef57-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="2ef57-129">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2ef57-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="2ef57-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ef57-130">Property</span></span>|<span data-ttu-id="2ef57-131">種類</span><span class="sxs-lookup"><span data-stu-id="2ef57-131">Type</span></span>|<span data-ttu-id="2ef57-132">説明</span><span class="sxs-lookup"><span data-stu-id="2ef57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ef57-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef57-133">displayName</span></span>|<span data-ttu-id="2ef57-134">String</span><span class="sxs-lookup"><span data-stu-id="2ef57-134">String</span></span>|<span data-ttu-id="2ef57-135">操作名。</span><span class="sxs-lookup"><span data-stu-id="2ef57-135">The operation name.</span></span>|
|<span data-ttu-id="2ef57-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ef57-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ef57-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ef57-137">DateTimeOffset</span></span>|<span data-ttu-id="2ef57-138">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="2ef57-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="2ef57-139">state</span><span class="sxs-lookup"><span data-stu-id="2ef57-139">state</span></span>|<span data-ttu-id="2ef57-140">String</span><span class="sxs-lookup"><span data-stu-id="2ef57-140">String</span></span>|<span data-ttu-id="2ef57-141">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="2ef57-141">The current state of the operation</span></span>|
|<span data-ttu-id="2ef57-142">id</span><span class="sxs-lookup"><span data-stu-id="2ef57-142">id</span></span>|<span data-ttu-id="2ef57-143">String</span><span class="sxs-lookup"><span data-stu-id="2ef57-143">String</span></span>|<span data-ttu-id="2ef57-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ef57-144">Key of the entity.</span></span>|
|<span data-ttu-id="2ef57-145">version</span><span class="sxs-lookup"><span data-stu-id="2ef57-145">version</span></span>|<span data-ttu-id="2ef57-146">String</span><span class="sxs-lookup"><span data-stu-id="2ef57-146">String</span></span>|<span data-ttu-id="2ef57-147">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ef57-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2ef57-148">応答</span><span class="sxs-lookup"><span data-stu-id="2ef57-148">Response</span></span>
<span data-ttu-id="2ef57-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ef57-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef57-150">例</span><span class="sxs-lookup"><span data-stu-id="2ef57-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ef57-151">要求</span><span class="sxs-lookup"><span data-stu-id="2ef57-151">Request</span></span>
<span data-ttu-id="2ef57-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ef57-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="2ef57-153">応答</span><span class="sxs-lookup"><span data-stu-id="2ef57-153">Response</span></span>
<span data-ttu-id="2ef57-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ef57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





