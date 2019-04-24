---
title: mobileAppDependency を作成する
description: 新しい mobileAppDependency オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85aeae1d8d76b4c4609ff38f1263aaeb9a634e9f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489059"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="6b31f-103">mobileAppDependency を作成する</span><span class="sxs-lookup"><span data-stu-id="6b31f-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="6b31f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b31f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b31f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b31f-106">新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b31f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b31f-107">Prerequisites</span></span>
<span data-ttu-id="6b31f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b31f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b31f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b31f-110">Permission type</span></span>|<span data-ttu-id="6b31f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b31f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b31f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b31f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b31f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b31f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b31f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b31f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b31f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b31f-115">Not supported.</span></span>|
|<span data-ttu-id="6b31f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b31f-116">Application</span></span>|<span data-ttu-id="6b31f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b31f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b31f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b31f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="6b31f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b31f-119">Request headers</span></span>
|<span data-ttu-id="6b31f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b31f-120">Header</span></span>|<span data-ttu-id="6b31f-121">値</span><span class="sxs-lookup"><span data-stu-id="6b31f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b31f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b31f-122">Authorization</span></span>|<span data-ttu-id="6b31f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b31f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6b31f-124">Accept</span></span>|<span data-ttu-id="6b31f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b31f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b31f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b31f-126">Request body</span></span>
<span data-ttu-id="6b31f-127">要求本文で、mobileAppDependency オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="6b31f-128">次の表に、mobileAppDependency の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="6b31f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b31f-129">Property</span></span>|<span data-ttu-id="6b31f-130">型</span><span class="sxs-lookup"><span data-stu-id="6b31f-130">Type</span></span>|<span data-ttu-id="6b31f-131">説明</span><span class="sxs-lookup"><span data-stu-id="6b31f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b31f-132">id</span><span class="sxs-lookup"><span data-stu-id="6b31f-132">id</span></span>|<span data-ttu-id="6b31f-133">String</span><span class="sxs-lookup"><span data-stu-id="6b31f-133">String</span></span>|<span data-ttu-id="6b31f-134">リレーションシップエンティティ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="6b31f-135">targetId</span><span class="sxs-lookup"><span data-stu-id="6b31f-135">targetId</span></span>|<span data-ttu-id="6b31f-136">String</span><span class="sxs-lookup"><span data-stu-id="6b31f-136">String</span></span>|<span data-ttu-id="6b31f-137">ターゲットの子モバイルアプリのアプリ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="6b31f-138">targetdisplayname</span><span class="sxs-lookup"><span data-stu-id="6b31f-138">targetDisplayName</span></span>|<span data-ttu-id="6b31f-139">String</span><span class="sxs-lookup"><span data-stu-id="6b31f-139">String</span></span>|<span data-ttu-id="6b31f-140">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="6b31f-140">The target child mobile app's display name.</span></span> <span data-ttu-id="6b31f-141">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="6b31f-142">dependencytype</span><span class="sxs-lookup"><span data-stu-id="6b31f-142">dependencyType</span></span>|[<span data-ttu-id="6b31f-143">mobileAppDependecyType</span><span class="sxs-lookup"><span data-stu-id="6b31f-143">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="6b31f-144">親アプリと子アプリ間の依存関係の種類。</span><span class="sxs-lookup"><span data-stu-id="6b31f-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="6b31f-145">可能な値は、`detect`、`autoInstall` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="6b31f-146">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="6b31f-146">dependentAppCount</span></span>|<span data-ttu-id="6b31f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6b31f-147">Int32</span></span>|<span data-ttu-id="6b31f-148">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="6b31f-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="6b31f-149">応答</span><span class="sxs-lookup"><span data-stu-id="6b31f-149">Response</span></span>
<span data-ttu-id="6b31f-150">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b31f-151">例</span><span class="sxs-lookup"><span data-stu-id="6b31f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b31f-152">要求</span><span class="sxs-lookup"><span data-stu-id="6b31f-152">Request</span></span>
<span data-ttu-id="6b31f-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b31f-154">応答</span><span class="sxs-lookup"><span data-stu-id="6b31f-154">Response</span></span>
<span data-ttu-id="6b31f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b31f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





