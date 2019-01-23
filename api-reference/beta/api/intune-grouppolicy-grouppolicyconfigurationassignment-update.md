---
title: GroupPolicyConfigurationAssignment を更新します。
description: GroupPolicyConfigurationAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08ff87b70b833dc1f8423a8465b5b880660fd462
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431652"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="b9c51-103">GroupPolicyConfigurationAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="b9c51-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="b9c51-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b9c51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b9c51-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9c51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9c51-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9c51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c51-107">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9c51-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c51-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9c51-108">Prerequisites</span></span>
<span data-ttu-id="b9c51-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9c51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9c51-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9c51-111">Permission type</span></span>|<span data-ttu-id="b9c51-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9c51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c51-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9c51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c51-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c51-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9c51-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9c51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c51-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9c51-116">Not supported.</span></span>|
|<span data-ttu-id="b9c51-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9c51-117">Application</span></span>|<span data-ttu-id="b9c51-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9c51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c51-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9c51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9c51-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9c51-120">Request headers</span></span>
|<span data-ttu-id="b9c51-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9c51-121">Header</span></span>|<span data-ttu-id="b9c51-122">値</span><span class="sxs-lookup"><span data-stu-id="b9c51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c51-123">Authorization</span></span>|<span data-ttu-id="b9c51-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b9c51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c51-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9c51-125">Accept</span></span>|<span data-ttu-id="b9c51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c51-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9c51-127">Request body</span></span>
<span data-ttu-id="b9c51-128">要求の本文に[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9c51-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b9c51-129">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b9c51-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="b9c51-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9c51-130">Property</span></span>|<span data-ttu-id="b9c51-131">型</span><span class="sxs-lookup"><span data-stu-id="b9c51-131">Type</span></span>|<span data-ttu-id="b9c51-132">説明</span><span class="sxs-lookup"><span data-stu-id="b9c51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c51-133">id</span><span class="sxs-lookup"><span data-stu-id="b9c51-133">id</span></span>|<span data-ttu-id="b9c51-134">String</span><span class="sxs-lookup"><span data-stu-id="b9c51-134">String</span></span>|<span data-ttu-id="b9c51-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b9c51-135">Key of the entity.</span></span>|
|<span data-ttu-id="b9c51-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c51-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b9c51-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c51-137">DateTimeOffset</span></span>|<span data-ttu-id="b9c51-138">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="b9c51-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="b9c51-139">target</span><span class="sxs-lookup"><span data-stu-id="b9c51-139">target</span></span>|[<span data-ttu-id="b9c51-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b9c51-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b9c51-141">グループの種類は、グループ ポリシーの構成を対象とします。</span><span class="sxs-lookup"><span data-stu-id="b9c51-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="b9c51-142">応答</span><span class="sxs-lookup"><span data-stu-id="b9c51-142">Response</span></span>
<span data-ttu-id="b9c51-143">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b9c51-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c51-144">例</span><span class="sxs-lookup"><span data-stu-id="b9c51-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c51-145">要求</span><span class="sxs-lookup"><span data-stu-id="b9c51-145">Request</span></span>
<span data-ttu-id="b9c51-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9c51-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b9c51-147">応答</span><span class="sxs-lookup"><span data-stu-id="b9c51-147">Response</span></span>
<span data-ttu-id="b9c51-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9c51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




