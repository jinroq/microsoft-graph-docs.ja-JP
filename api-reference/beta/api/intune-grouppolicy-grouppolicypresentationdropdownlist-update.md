---
title: GroupPolicyPresentationDropdownList を更新します。
description: GroupPolicyPresentationDropdownList オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cb39764767eba6bda56c4763660f7981f0e71db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430501"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="0d5fe-103">GroupPolicyPresentationDropdownList を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="0d5fe-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d5fe-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d5fe-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d5fe-107">[GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d5fe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d5fe-108">Prerequisites</span></span>
<span data-ttu-id="0d5fe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d5fe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d5fe-111">Permission type</span></span>|<span data-ttu-id="0d5fe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d5fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d5fe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d5fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d5fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d5fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0d5fe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d5fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d5fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-116">Not supported.</span></span>|
|<span data-ttu-id="0d5fe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d5fe-117">Application</span></span>|<span data-ttu-id="0d5fe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d5fe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d5fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="0d5fe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d5fe-120">Request headers</span></span>
|<span data-ttu-id="0d5fe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d5fe-121">Header</span></span>|<span data-ttu-id="0d5fe-122">値</span><span class="sxs-lookup"><span data-stu-id="0d5fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d5fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d5fe-123">Authorization</span></span>|<span data-ttu-id="0d5fe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d5fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d5fe-125">Accept</span></span>|<span data-ttu-id="0d5fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d5fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d5fe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d5fe-127">Request body</span></span>
<span data-ttu-id="0d5fe-128">要求の本文に[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="0d5fe-129">[GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="0d5fe-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d5fe-130">Property</span></span>|<span data-ttu-id="0d5fe-131">型</span><span class="sxs-lookup"><span data-stu-id="0d5fe-131">Type</span></span>|<span data-ttu-id="0d5fe-132">説明</span><span class="sxs-lookup"><span data-stu-id="0d5fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d5fe-133">label</span><span class="sxs-lookup"><span data-stu-id="0d5fe-133">label</span></span>|<span data-ttu-id="0d5fe-134">String</span><span class="sxs-lookup"><span data-stu-id="0d5fe-134">String</span></span>|<span data-ttu-id="0d5fe-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0d5fe-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-136">The default value is empty.</span></span> <span data-ttu-id="0d5fe-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0d5fe-138">id</span><span class="sxs-lookup"><span data-stu-id="0d5fe-138">id</span></span>|<span data-ttu-id="0d5fe-139">String</span><span class="sxs-lookup"><span data-stu-id="0d5fe-139">String</span></span>|<span data-ttu-id="0d5fe-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-140">Key of the entity.</span></span> <span data-ttu-id="0d5fe-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0d5fe-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d5fe-142">lastModifiedDateTime</span></span>|<span data-ttu-id="0d5fe-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d5fe-143">DateTimeOffset</span></span>|<span data-ttu-id="0d5fe-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="0d5fe-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0d5fe-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="0d5fe-146">defaultItem</span></span>|[<span data-ttu-id="0d5fe-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="0d5fe-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="0d5fe-148">項目のリストの既定の選択肢を識別する文字列値をローカライズします。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="0d5fe-149">items</span><span class="sxs-lookup"><span data-stu-id="0d5fe-149">items</span></span>|<span data-ttu-id="0d5fe-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d5fe-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="0d5fe-151">一連のローカライズされた表示名とその値を表します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="0d5fe-152">必須</span><span class="sxs-lookup"><span data-stu-id="0d5fe-152">required</span></span>|<span data-ttu-id="0d5fe-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d5fe-153">Boolean</span></span>|<span data-ttu-id="0d5fe-154">パラメーター] ボックスに値を入力するための要件です。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="0d5fe-155">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="0d5fe-156">応答</span><span class="sxs-lookup"><span data-stu-id="0d5fe-156">Response</span></span>
<span data-ttu-id="0d5fe-157">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d5fe-158">例</span><span class="sxs-lookup"><span data-stu-id="0d5fe-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d5fe-159">要求</span><span class="sxs-lookup"><span data-stu-id="0d5fe-159">Request</span></span>
<span data-ttu-id="0d5fe-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="0d5fe-161">応答</span><span class="sxs-lookup"><span data-stu-id="0d5fe-161">Response</span></span>
<span data-ttu-id="0d5fe-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d5fe-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```




