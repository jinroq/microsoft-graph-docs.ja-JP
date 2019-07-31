---
title: GroupPolicyConfigurationAssignment の更新
description: GroupPolicyConfigurationAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cc10a34cd4c2482fc72c4e73fc6efda0f320e26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989974"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="b8a08-103">GroupPolicyConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b8a08-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="b8a08-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8a08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a08-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8a08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a08-106">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8a08-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8a08-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b8a08-107">Prerequisites</span></span>
<span data-ttu-id="b8a08-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8a08-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8a08-110">Permission type</span></span>|<span data-ttu-id="b8a08-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8a08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8a08-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8a08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8a08-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a08-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8a08-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8a08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8a08-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8a08-115">Not supported.</span></span>|
|<span data-ttu-id="b8a08-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8a08-116">Application</span></span>|<span data-ttu-id="b8a08-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8a08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8a08-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8a08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b8a08-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8a08-119">Request headers</span></span>
|<span data-ttu-id="b8a08-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8a08-120">Header</span></span>|<span data-ttu-id="b8a08-121">値</span><span class="sxs-lookup"><span data-stu-id="b8a08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8a08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8a08-122">Authorization</span></span>|<span data-ttu-id="b8a08-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8a08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8a08-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b8a08-124">Accept</span></span>|<span data-ttu-id="b8a08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8a08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8a08-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8a08-126">Request body</span></span>
<span data-ttu-id="b8a08-127">要求本文で、 [Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8a08-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b8a08-128">次の表に、 [Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b8a08-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="b8a08-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8a08-129">Property</span></span>|<span data-ttu-id="b8a08-130">型</span><span class="sxs-lookup"><span data-stu-id="b8a08-130">Type</span></span>|<span data-ttu-id="b8a08-131">説明</span><span class="sxs-lookup"><span data-stu-id="b8a08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a08-132">id</span><span class="sxs-lookup"><span data-stu-id="b8a08-132">id</span></span>|<span data-ttu-id="b8a08-133">String</span><span class="sxs-lookup"><span data-stu-id="b8a08-133">String</span></span>|<span data-ttu-id="b8a08-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b8a08-134">Key of the entity.</span></span>|
|<span data-ttu-id="b8a08-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8a08-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b8a08-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8a08-136">DateTimeOffset</span></span>|<span data-ttu-id="b8a08-137">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="b8a08-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="b8a08-138">target</span><span class="sxs-lookup"><span data-stu-id="b8a08-138">target</span></span>|[<span data-ttu-id="b8a08-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b8a08-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b8a08-140">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="b8a08-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="b8a08-141">応答</span><span class="sxs-lookup"><span data-stu-id="b8a08-141">Response</span></span>
<span data-ttu-id="b8a08-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8a08-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8a08-143">例</span><span class="sxs-lookup"><span data-stu-id="b8a08-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8a08-144">要求</span><span class="sxs-lookup"><span data-stu-id="b8a08-144">Request</span></span>
<span data-ttu-id="b8a08-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8a08-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8a08-146">応答</span><span class="sxs-lookup"><span data-stu-id="b8a08-146">Response</span></span>
<span data-ttu-id="b8a08-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b8a08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





