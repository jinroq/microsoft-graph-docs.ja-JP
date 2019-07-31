---
title: educationSynchronizationProfile リソースの種類
description: 教育機関のエンティティおよび名簿の情報をソースディレクトリから Azure Active Directory (Azure AD) に同期するために使用される構成のセットを表します。 このリソースは、School Data Sync で使用されるプログラム的な表現を提供します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5d79c50d29d4a89aa78b724f7cde747ea90706b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972356"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教育機関のエンティティおよび名簿の情報をソースディレクトリから Azure Active Directory (Azure AD) に同期するために使用される構成のセットを表します。 このリソースは、 [School Data Sync](https://sds.microsoft.com)で使用されるプログラム的な表現を提供します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期プロファイルの一覧表示](../api/educationsynchronizationprofile-list.md) | **educationSynchronizationProfile**コレクション | テナント内のすべての同期プロファイルの一覧を取得します。 |
| [同期プロファイルを取得する](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | プロファイル識別子を指定して、特定のプロファイルを取得します。 |
| [同期プロファイルの作成](../api/educationsynchronizationprofile-post.md) | None | 新しい同期プロファイルを作成します。 |
| [同期プロファイルの削除](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | プロファイル識別子を指定して、特定のプロファイルを削除します。 |
| [進行中の同期を一時停止する](../api/educationsynchronizationprofile-pause.md) | None | 進行中の同期を一時停止します。 |
| [一時停止した同期を再開する](../api/educationsynchronizationprofile-resume.md) | None | 一時停止した同期を再開します。 |
| [同期をリセットする](../api/educationsynchronizationprofile-reset.md) | None | プロファイルの状態をリセットし、同期を再開します。 |
| [アップロードしたファイルの同期を開始する](../api/educationsynchronizationprofile-start.md) | [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)コレクション| アップロードしたソースファイルを確認し、同期を開始します。 データプロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)の場合にのみ適用されます。 |
| [アップロード URL を取得する](../api/educationsynchronizationprofile-uploadurl.md) | string | CSV データファイルをアップロードするための短時間の URL を返します。 データプロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)の場合にのみ適用されます。 |
| [同期の状態を取得する](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | 特定の同期プロファイルの状態を返します。 |
| [同期エラーを取得する](../api/educationsynchronizationerrors-get.md) | [educationSynchronizationError](educationsynchronizationerror.md)コレクション| 同期中に生成されたすべてのエラーを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **displayName** | string |  Id を同期するための構成プロファイルの名前。         |
| **プロバイダー** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  プロファイルに使用されるデータプロバイダー。         |
| **id の同期構成** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | Id の[作成](educationidentitycreationconfiguration.md)または[一致する](educationidentitymatchingconfiguration.md)構成。        |
| **licensesToAssign** | [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)コレクション|  ライセンスのセットアップ構成。        |
| **state** | educationSynchronizationProfileState |  プロファイルの状態。 可能な値は、`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed` です。          |

## <a name="relationships"></a>リレーションシップ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **errors** | [educationSynchronizationError](educationsynchronizationerror.md)コレクション| この同期プロファイルに関連付けられているすべてのエラー。 |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | 同期の状態。 |

## <a name="json-representation"></a>JSON 表記
次に示すのは、 **educationSynchronizationProfile**リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "id": "String",
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
