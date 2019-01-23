---
title: GroupPolicyConfigurationAssignment を作成します。
description: 新しい groupPolicyConfigurationAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db4c96db45f5c54f70cf1216829834b453dbcd9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430500"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="fef38-103">GroupPolicyConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="fef38-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="fef38-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fef38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fef38-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fef38-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fef38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef38-107">新しい[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fef38-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fef38-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fef38-108">Prerequisites</span></span>
<span data-ttu-id="fef38-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fef38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fef38-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fef38-111">Permission type</span></span>|<span data-ttu-id="fef38-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fef38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef38-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fef38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fef38-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef38-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fef38-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fef38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef38-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef38-116">Not supported.</span></span>|
|<span data-ttu-id="fef38-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fef38-117">Application</span></span>|<span data-ttu-id="fef38-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef38-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fef38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fef38-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fef38-120">Request headers</span></span>
|<span data-ttu-id="fef38-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fef38-121">Header</span></span>|<span data-ttu-id="fef38-122">値</span><span class="sxs-lookup"><span data-stu-id="fef38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fef38-123">Authorization</span></span>|<span data-ttu-id="fef38-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fef38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fef38-125">Accept</span></span>|<span data-ttu-id="fef38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fef38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef38-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fef38-127">Request body</span></span>
<span data-ttu-id="fef38-128">要求の本文に groupPolicyConfigurationAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fef38-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="fef38-129">次の表は、groupPolicyConfigurationAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fef38-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="fef38-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef38-130">Property</span></span>|<span data-ttu-id="fef38-131">型</span><span class="sxs-lookup"><span data-stu-id="fef38-131">Type</span></span>|<span data-ttu-id="fef38-132">説明</span><span class="sxs-lookup"><span data-stu-id="fef38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef38-133">id</span><span class="sxs-lookup"><span data-stu-id="fef38-133">id</span></span>|<span data-ttu-id="fef38-134">String</span><span class="sxs-lookup"><span data-stu-id="fef38-134">String</span></span>|<span data-ttu-id="fef38-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fef38-135">Key of the entity.</span></span>|
|<span data-ttu-id="fef38-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fef38-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fef38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fef38-137">DateTimeOffset</span></span>|<span data-ttu-id="fef38-138">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="fef38-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="fef38-139">target</span><span class="sxs-lookup"><span data-stu-id="fef38-139">target</span></span>|[<span data-ttu-id="fef38-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fef38-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fef38-141">グループの種類は、グループ ポリシーの構成を対象とします。</span><span class="sxs-lookup"><span data-stu-id="fef38-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fef38-142">応答</span><span class="sxs-lookup"><span data-stu-id="fef38-142">Response</span></span>
<span data-ttu-id="fef38-143">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fef38-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef38-144">例</span><span class="sxs-lookup"><span data-stu-id="fef38-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef38-145">要求</span><span class="sxs-lookup"><span data-stu-id="fef38-145">Request</span></span>
<span data-ttu-id="fef38-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fef38-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="fef38-147">応答</span><span class="sxs-lookup"><span data-stu-id="fef38-147">Response</span></span>
<span data-ttu-id="fef38-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fef38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




