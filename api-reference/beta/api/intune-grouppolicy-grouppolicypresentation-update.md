---
title: GroupPolicyPresentation を更新します。
description: GroupPolicyPresentation オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 26f185d1474402f77f8dab09c500a1c11892f77b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431612"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="58e57-103">GroupPolicyPresentation を更新します。</span><span class="sxs-lookup"><span data-stu-id="58e57-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="58e57-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58e57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58e57-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58e57-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58e57-107">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58e57-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58e57-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="58e57-108">Prerequisites</span></span>
<span data-ttu-id="58e57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58e57-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58e57-111">Permission type</span></span>|<span data-ttu-id="58e57-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="58e57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58e57-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58e57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58e57-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e57-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58e57-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58e57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58e57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e57-116">Not supported.</span></span>|
|<span data-ttu-id="58e57-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58e57-117">Application</span></span>|<span data-ttu-id="58e57-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58e57-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58e57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="58e57-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58e57-120">Request headers</span></span>
|<span data-ttu-id="58e57-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58e57-121">Header</span></span>|<span data-ttu-id="58e57-122">値</span><span class="sxs-lookup"><span data-stu-id="58e57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58e57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e57-123">Authorization</span></span>|<span data-ttu-id="58e57-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="58e57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58e57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58e57-125">Accept</span></span>|<span data-ttu-id="58e57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58e57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58e57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="58e57-127">Request body</span></span>
<span data-ttu-id="58e57-128">要求の本文に[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="58e57-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="58e57-129">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="58e57-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="58e57-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58e57-130">Property</span></span>|<span data-ttu-id="58e57-131">型</span><span class="sxs-lookup"><span data-stu-id="58e57-131">Type</span></span>|<span data-ttu-id="58e57-132">説明</span><span class="sxs-lookup"><span data-stu-id="58e57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58e57-133">label</span><span class="sxs-lookup"><span data-stu-id="58e57-133">label</span></span>|<span data-ttu-id="58e57-134">String</span><span class="sxs-lookup"><span data-stu-id="58e57-134">String</span></span>|<span data-ttu-id="58e57-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="58e57-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="58e57-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="58e57-136">The default value is empty.</span></span>|
|<span data-ttu-id="58e57-137">id</span><span class="sxs-lookup"><span data-stu-id="58e57-137">id</span></span>|<span data-ttu-id="58e57-138">String</span><span class="sxs-lookup"><span data-stu-id="58e57-138">String</span></span>|<span data-ttu-id="58e57-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="58e57-139">Key of the entity.</span></span>|
|<span data-ttu-id="58e57-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58e57-140">lastModifiedDateTime</span></span>|<span data-ttu-id="58e57-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e57-141">DateTimeOffset</span></span>|<span data-ttu-id="58e57-142">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="58e57-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="58e57-143">応答</span><span class="sxs-lookup"><span data-stu-id="58e57-143">Response</span></span>
<span data-ttu-id="58e57-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="58e57-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e57-145">例</span><span class="sxs-lookup"><span data-stu-id="58e57-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="58e57-146">要求</span><span class="sxs-lookup"><span data-stu-id="58e57-146">Request</span></span>
<span data-ttu-id="58e57-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58e57-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="58e57-148">応答</span><span class="sxs-lookup"><span data-stu-id="58e57-148">Response</span></span>
<span data-ttu-id="58e57-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58e57-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




