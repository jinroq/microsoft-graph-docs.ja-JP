---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6848e9f4d397163437d133fbe4f9446a7278680
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994790"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="514b8-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="514b8-103">Create managedAppOperation</span></span>

> <span data-ttu-id="514b8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="514b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="514b8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="514b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="514b8-106">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="514b8-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="514b8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="514b8-107">Prerequisites</span></span>
<span data-ttu-id="514b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="514b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="514b8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="514b8-110">Permission type</span></span>|<span data-ttu-id="514b8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="514b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="514b8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="514b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="514b8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514b8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="514b8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="514b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="514b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="514b8-115">Not supported.</span></span>|
|<span data-ttu-id="514b8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="514b8-116">Application</span></span>|<span data-ttu-id="514b8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="514b8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="514b8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="514b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="514b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="514b8-119">Request headers</span></span>
|<span data-ttu-id="514b8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="514b8-120">Header</span></span>|<span data-ttu-id="514b8-121">値</span><span class="sxs-lookup"><span data-stu-id="514b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="514b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="514b8-122">Authorization</span></span>|<span data-ttu-id="514b8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="514b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="514b8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="514b8-124">Accept</span></span>|<span data-ttu-id="514b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="514b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="514b8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="514b8-126">Request body</span></span>
<span data-ttu-id="514b8-127">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="514b8-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="514b8-128">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="514b8-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="514b8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="514b8-129">Property</span></span>|<span data-ttu-id="514b8-130">型</span><span class="sxs-lookup"><span data-stu-id="514b8-130">Type</span></span>|<span data-ttu-id="514b8-131">説明</span><span class="sxs-lookup"><span data-stu-id="514b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="514b8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="514b8-132">displayName</span></span>|<span data-ttu-id="514b8-133">String</span><span class="sxs-lookup"><span data-stu-id="514b8-133">String</span></span>|<span data-ttu-id="514b8-134">操作名。</span><span class="sxs-lookup"><span data-stu-id="514b8-134">The operation name.</span></span>|
|<span data-ttu-id="514b8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="514b8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="514b8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="514b8-136">DateTimeOffset</span></span>|<span data-ttu-id="514b8-137">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="514b8-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="514b8-138">state</span><span class="sxs-lookup"><span data-stu-id="514b8-138">state</span></span>|<span data-ttu-id="514b8-139">String</span><span class="sxs-lookup"><span data-stu-id="514b8-139">String</span></span>|<span data-ttu-id="514b8-140">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="514b8-140">The current state of the operation</span></span>|
|<span data-ttu-id="514b8-141">id</span><span class="sxs-lookup"><span data-stu-id="514b8-141">id</span></span>|<span data-ttu-id="514b8-142">文字列</span><span class="sxs-lookup"><span data-stu-id="514b8-142">String</span></span>|<span data-ttu-id="514b8-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="514b8-143">Key of the entity.</span></span>|
|<span data-ttu-id="514b8-144">version</span><span class="sxs-lookup"><span data-stu-id="514b8-144">version</span></span>|<span data-ttu-id="514b8-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="514b8-145">String</span></span>|<span data-ttu-id="514b8-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="514b8-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="514b8-147">応答</span><span class="sxs-lookup"><span data-stu-id="514b8-147">Response</span></span>
<span data-ttu-id="514b8-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="514b8-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="514b8-149">例</span><span class="sxs-lookup"><span data-stu-id="514b8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="514b8-150">要求</span><span class="sxs-lookup"><span data-stu-id="514b8-150">Request</span></span>
<span data-ttu-id="514b8-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="514b8-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="514b8-152">応答</span><span class="sxs-lookup"><span data-stu-id="514b8-152">Response</span></span>
<span data-ttu-id="514b8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="514b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





