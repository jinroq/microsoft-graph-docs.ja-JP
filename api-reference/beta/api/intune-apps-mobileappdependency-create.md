---
title: MobileAppDependency を作成する
description: 新しい mobileAppDependency オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69ff12bb7c0d00457d86d62c467778de2a9223fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329181"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="40429-103">MobileAppDependency を作成する</span><span class="sxs-lookup"><span data-stu-id="40429-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="40429-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40429-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40429-106">新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="40429-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40429-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="40429-107">Prerequisites</span></span>
<span data-ttu-id="40429-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40429-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40429-110">Permission type</span></span>|<span data-ttu-id="40429-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40429-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40429-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40429-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40429-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40429-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40429-115">Not supported.</span></span>|
|<span data-ttu-id="40429-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40429-116">Application</span></span>|<span data-ttu-id="40429-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40429-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40429-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="40429-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40429-119">Request headers</span></span>
|<span data-ttu-id="40429-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40429-120">Header</span></span>|<span data-ttu-id="40429-121">値</span><span class="sxs-lookup"><span data-stu-id="40429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40429-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40429-122">Authorization</span></span>|<span data-ttu-id="40429-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="40429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40429-124">承諾</span><span class="sxs-lookup"><span data-stu-id="40429-124">Accept</span></span>|<span data-ttu-id="40429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40429-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40429-126">Request body</span></span>
<span data-ttu-id="40429-127">要求本文で、mobileAppDependency オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40429-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="40429-128">次の表に、mobileAppDependency の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="40429-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="40429-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40429-129">Property</span></span>|<span data-ttu-id="40429-130">型</span><span class="sxs-lookup"><span data-stu-id="40429-130">Type</span></span>|<span data-ttu-id="40429-131">説明</span><span class="sxs-lookup"><span data-stu-id="40429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40429-132">id</span><span class="sxs-lookup"><span data-stu-id="40429-132">id</span></span>|<span data-ttu-id="40429-133">String</span><span class="sxs-lookup"><span data-stu-id="40429-133">String</span></span>|<span data-ttu-id="40429-134">リレーションシップエンティティ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40429-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="40429-135">targetId</span><span class="sxs-lookup"><span data-stu-id="40429-135">targetId</span></span>|<span data-ttu-id="40429-136">String</span><span class="sxs-lookup"><span data-stu-id="40429-136">String</span></span>|<span data-ttu-id="40429-137">ターゲットの子モバイルアプリのアプリ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40429-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="40429-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="40429-138">targetDisplayName</span></span>|<span data-ttu-id="40429-139">String</span><span class="sxs-lookup"><span data-stu-id="40429-139">String</span></span>|<span data-ttu-id="40429-140">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="40429-140">The target child mobile app's display name.</span></span> <span data-ttu-id="40429-141">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40429-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="40429-142">dependencyType</span><span class="sxs-lookup"><span data-stu-id="40429-142">dependencyType</span></span>|[<span data-ttu-id="40429-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="40429-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="40429-144">親アプリと子アプリ間の依存関係の種類。</span><span class="sxs-lookup"><span data-stu-id="40429-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="40429-145">可能な値は、`detect`、`autoInstall` です。</span><span class="sxs-lookup"><span data-stu-id="40429-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="40429-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="40429-146">dependentAppCount</span></span>|<span data-ttu-id="40429-147">Int32</span><span class="sxs-lookup"><span data-stu-id="40429-147">Int32</span></span>|<span data-ttu-id="40429-148">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="40429-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="40429-149">応答</span><span class="sxs-lookup"><span data-stu-id="40429-149">Response</span></span>
<span data-ttu-id="40429-150">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40429-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40429-151">例</span><span class="sxs-lookup"><span data-stu-id="40429-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="40429-152">要求</span><span class="sxs-lookup"><span data-stu-id="40429-152">Request</span></span>
<span data-ttu-id="40429-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40429-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="40429-154">応答</span><span class="sxs-lookup"><span data-stu-id="40429-154">Response</span></span>
<span data-ttu-id="40429-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40429-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```






