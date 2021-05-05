# qe-rancher

QE Rancher - Repository for scheduling & scripts & documentation

## Scheduling Rancher tests on openqa.opensuse.org
 * File [.github/workflows/o3_schedule.yaml](.github/workflows/o3_schedule.yaml)
 * Automatically scheduled **every Monday on 6AM**
 * Manually scheduled when pushing to **o3_schedule** branch
 * Results apear in [openqa.opensuse.org](https://openqa.opensuse.org/group_overview/78)

## Useful commands
 * Latest O3 Tumbleweed awailable image:
   ```bash
   curl -s https://openqa.opensuse.org/group_overview/1.json| jq -r '[.build_results[] | select(.tag.description=="published") | select(.version=="Tumbleweed") | .build] | sort | reverse | .[0]'
   ```

## Authors
 * [Pavel Dostál](http://github.com/pdostal)
 * [George Gkioulis](https://github.com/ggkioulis)
 * [Anna Minou](http://github.com/punkioudi)
 * [Ivan Lausuch](https://github.com/ilausuch)
 
